
# Writer/Designer's studio: web unit

**Work to have done**:

* As much of the [Interneting is Hard](https://internetingishard.com/html-and-css/) [(but at least it's WebArchive crawled)](https://web.archive.org/web/20201105195453/https://www.internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors")
* More on CSS selectors: the [CSS Diner](https://flukeout.github.io/) game and/or [a CSS-Tricks roundup](https://css-tricks.com/how-css-selectors-work/)
* A website proposal, posted to the [Issue Queue]({{site.github.issues_url}}/)


**Plan for the day**:
1. General advice on moving from proposal to product <!-- Don't open all of these! Just read the headlines, and get into the inspector demo. -->
2. Brief intro to the browser inspector (Firefox, Chrome)
3. Set goals and go forth!
4. Update your goals


## 1. Here's what you need to know today

### Beware of scope creep; plan for phased releases

Bear in mind that you only have a couple more weeks on this project. If you've just given yourself an ambitious agenda, think about "minimum deliverable product" and "stretch goals." You have version control; you can iterate. In other words: you can always come back and add *more*, but it's good to start with what's really at the *core* of your website idea.

### Start by thinking about structure (i.e. HTML before CSS)

Remember from last time that though you probably have a vision for how your site should _look_, it makes sense to **begin by thinking about the _structure of your content_**. That will give you the material you need to support _multiple_ views, depending on screen size and/or what begins to feel most important.</p>

So I recommend starting by listing and grouping:

1. What are the content sections your site will include?
2. How might you group those things hierarchically? That is, what's the most important for a viewer to encounter first? Which things are (or could be) parts of others, and which things have to be at the same level?
3. If you can make a nested list of your content areas, that could serve you as a navigation... and probably also a list of headers (`h1`, `h2`, etc).


### You don't have to reinvent the wheel

Like other kinds of media, web design has its genres... and certain _genre conventions_ that solve recurring design problems. You can find some of these by looking at the code of websites you like: you can right-click on any page and choose **"View Page Source"** (or something like it) to see the full rendered HTML page. From there, you can also click the link in the `head` to see the full stylesheet.

<div class="alert alert-warning">NB: This works a lot better on simple, static sites than, say, an e-commerce site that's tracking your clicks in complex ways. But even there, you should be starting to get a sense of how to skim for the recurring chunks of markup.</div>

For instance, a very common structure you should all know about is this one:
```html
<nav class="main-nav" id="main-nav">
  <ul>
    <li class="active">
      <a href="/index.html">Home</a>
    </li>
    <li>
      <a href="/about.html">About the Author</a>
    </li>
    <li>
      <a href="/articles.html">Past Publications</a>
    </li>
    <!-- etc -->
    </ul>
  </nav>
```

You can then style that menu to your heart's content:

```css
  /***** Main menu styling *****/
  nav.main-nav {
    height: 3em;
  }

  nav.main-nav ul {
    list-style-type: none;
    display: flex;
  }

  nav.main-nav li {
    padding: 1em;
  }

  /* etc */
```


### When you're ready to work on appearances, test CSS rules directly in the browser

Viewing the full page source is great for seeing how professional designers organize their documents. But most of the time, you'll want to be more targeted: you don't _want_ to have to sift through everything just to figure out the color or font on that one blockquote or button (or whatever it is you want to imitate and thereby learn from).

Chrome and Firefox (especially Firefox) have great built-in developer tools to "inspect" elements of the page. It's already available: just **right-click anywhere and choose "inspect element"** to see the local html, the full cascade of CSS rules that apply to it, and a few other features beside.

<aside class="alert alert-info">Safari can do this, too, but you'll need to <a href="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html">activate it first</a>... and then "show the details sidebar."</aside>

<p>Crucially, you can also <em>add CSS rules</em> and immediately see what effect they would have on the page. (Safari users, note that the button to add a new rule is on the bottom left, not the top right as in the other two browsers.) Color pickers are an especially nice feature – and perhaps the one thing that Chrome's inspector does better than Firefox's at the moment, in that Chrome lets you change from hex color to RGBA or HSL, and directly adjust saturation / luminosity, e.g. to improve contrast.</p>

<figure role="figure">
<img src="../assets/img/inspect-element--firefox--skeleton.gif" alt="screencast of the firefox in-browser inspector" />
</figure>

Just be sure to **copy your changes to a file for safe keeping**, or they'll disappear when you refresh! To make copy/paste easier, click on the source your browser created for your new rules: in Firefox it's called "inline", in Chrome "inspector-stylesheet", in Safari "Inspector Stylesheet."



## 2. General advice on moving from proposal to product

In a moment, I'm going to invite you to set goals for studio time. If you haven't yet sorted out your navigation, that's a great place to start!

Here are some other things to consider as you move forward:

<details><summary>Your homepage should probably be called something like index.html</summary>

I'm going to recommend that everyone use GitHub Pages to publish your sites unless you have a good reason not to. (And you might; but talk to me about it.) In that system, you store your files in a GitHub repository (in a branch called "gh-pages," like this site, or a subdirectory called "docs" – look in your own repos!), and GH knows where to look to find your stuff. <em>By default, it'll show your README.md file as the home page, unless it finds a file called index.html or index.md</em>.

Therefore, rather than call your landing page myproject.html, landing.html, or home.html, you're better off using the index.html name. You can always change the <code>&lt;title&gt;</code> to give it a more accurate name in the browser tab. : )
</details>

<details><summary>Strive for semanticity.</summary>

Ask yourself:
<ul>
  <li>Can you tell what's going on just by reading the HTML file?</li>
  <li>Do your header levels (<code>&lt;h1&gt;, &lt;h2&gt;</code>, etc) correspond to your intended hierarchy? Try not to jump levels.</li>
  <li>Does the HTML hard-code any display (e.g. <code>&lt;center&gt;</code>, <code>&lt;b&gt;</code>) that should be in the CSS? (Older tutorials will suggest this, but it's not a great idea.)</li>
</ul>
</details>  

<details>
  <summary>Let appearances reflect the structure, not vice-versa</summary>
  <p>This one's related to what I said above, but applies especially when you're starting to think about appearances. <em>Visuals are volatile; structure should be steady.</em> It can be very tempting to just accept your browser's default styles as a given, e.g. to jump from a large <code>&lt;h1&gt;</code> page title to an <code>&lt;h5&gt;</code> subtitle because the latter "looks about right." But this would mis-represent the actual structure of the document – and would seriously confuse screen-reader software trying to present the page to a blind visitor. Instead, use your browser's Inspector to take note of the CSS rules defining that <code>&lt;h5&gt;</code>, and apply them to <code>&lt;h2&gt;</code> in your stylesheet.</p><!-- This makes a good jump-point into the inspector... -->
</details>

<details> <!-- CONSIDER: SHOULD WE DO THIS ALL TOGETHER? -->
<summary>Stuck for what to do, CSS-wise? Start with some basic spacing</summary>

<p>Work your way through <a href="http://jgthms.com/web-design-in-4-minutes">Web Design in 4 Minutes</a>, and borrow some of the most essential rules... e.g. <ul><li>set a maximum width for text</li><li>add padding on main content and headers</li><li>change font-family away from the default "Times"</li></ul></p>

<p>For more advanced layout (sidebars, columns, grids, etc), see the links in the homework assignment.</p>

</details>



<!-- FOR NEXT LESSON, not today

## 2. Other notes


* Take on the lowest line-count challenge. Ask yourself:
  - does that div need to be there?
  - could those CSS rules be combined?


  <details>
  <summary>Take advantage of parent selectors and classes to limit the scope of CSS rules</summary>
  <p>If you're worried a rule will spread too broadly, e.g. affecting inner page <code>&lt;h2&gt;</code>'s when you only meant it to apply on the front page, just limit the scope of the css rule by specifying a class, or a parent container, or both. For example, the following code will only apply to <code>&lt;h2&gt;</code>'s inside a <code>&lt;body class="front"&gt;</code>:
  <pre><code class="css">
  body.front h2 {
    font-size: 18px;
  }
  </code></pre>
  (Setting a class on the <code>&lt;body&gt;</code> is a good way to set up page-wide contexts, e.g. for background or the position of a navigation bar.)
  </p>
  <p>
  Or here's code that only applies to an <code>&lt;h2&gt;</code> when it appears inside an element (a <code>&lt;div&gt;</code>, say, or a <code>&lt;header&gt;</code>) with class "title-block":
  <pre><code class="css">
  .title-block h2 {
    font-size: 18px;
  }
  </code></pre>
  This solution probably makes the most sense if you want to do some styling on the containing element, like changing its background or centering a bunch of things.
  </p>
  <p>
  Or – probably the simplest solution of all – you could just set the class directly on the element, calling it something like "subtitle" (or whatever you want to call it): <pre><code class="html">&lt;h2 class="subtitle"&gt;</code></pre>
  <pre><code class="css">
  h2.subtitle {
    font-size: 18px;
  }
  </code></pre>

  This has the extra advantage that you can set a lot of other rules for <em>all</em> <code>&lt;h2&gt;</code>'s, and just add the tweaks you need for the subtitle in this additional ruleset. In other words: the Cascading Style Sheet will cascade!
  </p>
  </details>

-->

## 3. Go forth!

In the [shared google doc](http://bit.ly/cdm2021spring-notes), **set a goal for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project? Note that a Website Preview is due a week from today.

<div class="alert alert-info">
If you haven't yet, please do expand and read my notes above. Also remember that you have many <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website; for today, might I especially point out the <strong>design advantages of <a href="https://loremipsum.io">placeholder text</a> and/or <a href="https://loremipsum.io/21-of-the-best-placeholder-image-generators/">images</a></strong>?
</div>


<div class="alert alert-warning">
As usual, to get credit for asynchronous participation, please add your intentions and exit notes to the google doc when you start and stop working – and aim to work for at least two 20-minute pomodoros. <!-- (In class, we had about 50 minutes of straight-up studio time.) -->
</div>


Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

<strong>Reply to your note in the <a href="http://bit.ly/cdm2021spring-notes">google doc</a>.</strong>
</div>

# (No) homework for next time

No homework tonight! Tomorrow is a self-care day, and I sincerely hope you do something healing for yourselves.
