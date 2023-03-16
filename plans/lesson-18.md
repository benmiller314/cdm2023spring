
# Writer/Designer's studio: web unit

**Work to have done**:

* As much of the [Interneting is Hard](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors"), with exercises pushed to your repo's "tutorials" folder
* More on CSS selectors: the [CSS Diner](https://flukeout.github.io/) game and/or [a CSS-Tricks roundup](https://css-tricks.com/how-css-selectors-work/)



**Plan for the day**:
1. Threshold Concepts: what you all need to know
2. Ideas for studio <!-- Don't open all of these! Just read the headlines, and get into the inspector demo. -->
<!-- 2. Brief intro to the browser inspector (Firefox, Chrome) -->
3. Set goals and go forth!
4. Update your goals


## 1. Here's what you need to know today
<!--
### Beware of scope creep; plan for phased releases

Bear in mind that you only have a couple more weeks on this project. If you've just given yourself an ambitious agenda, think about "minimum deliverable product" and "stretch goals." You have version control; you can iterate. In other words: you can always come back and add *more*, but it's good to start with what's really at the *core* of your website idea. -->

### Start by thinking about structure (i.e. HTML before CSS)

Remember that though you probably have a vision for how your site should _look_, it makes sense to **begin by thinking about the _structure of your content_**. That will give you the material you need to support _multiple_ views, depending on screen size and/or what begins to feel most important.

So I recommend starting by listing and grouping:

1. What are the content sections your site will include?
2. How might you group those things hierarchically? That is, what's the most important for a viewer to encounter first? Which things are (or could be) parts of others, and which things have to be at the same level?
3. If you can make a nested list of your content areas, that could serve you as a navigation... and probably also a list of headers (`h1`, `h2`, etc).


### You don't have to reinvent the wheel

Like other kinds of media, web design has its genres... and certain _genre conventions_ that solve recurring design problems. You can find some of these by looking at the code of websites you like: you can right-click on any page and choose **"View Page Source"** (or something like it) to see the full rendered HTML page. From there, you can also click the link in the `head` to see the full stylesheet.

<div class="alert alert-warning">NB: This works a lot better on simple, static sites than, say, an e-commerce site that's tracking your clicks in complex ways. But even there, you should be starting to get a sense of how to skim for the recurring chunks of markup.</div>

For instance, a very common structure you should all know about is this one, for a basic navigation menu:
```html
<nav class="main-nav" id="main-nav">
  <ul>
    <li class="active"><a href="/index.html">Home</a></li>
    <li><a href="/about.html">About the Author</a></li>
    <li><a href="/articles.html">Past Publications</a></li>
    <!-- etc -->
  </ul>
</nav>
```

<div class="alert alert-success">
Let's look at this in a testing space: <a href="https://codepen.io/benmiller314/pen/xxpZrOY?editors=1100">https://codepen.io/benmiller314/pen/xxpZrOY?editors=1100</a>
</div>

Note that:

* The semantic element `<nav>` [automatically communicates](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/navigation_role) the navigation role to audio screen readers, helping blind users find their way around your site.
* We use list items so screen readers can easily enumerate the number of locations
* You can use a class like "active" to keep site visitors oriented within the space of your site. (There are other ways, too, but this is pretty simple.)

You can then style that menu to your heart's content:

```css
/***** Main menu styling *****/
  .main-nav {
    background-color: #eee; /* light gray */
  }

  .main-nav a {
    color: #4b8568;         /* dark green */
  }

  .main-nav ul {
    list-style-type: none;  /* Hide the bullets */
    display: flex;          /* Arrange horizontally, not vertically */
  }

  .main-nav li {
    padding: 1em 2em;           /* Add a little space around each link */
  }

  .main-nav .active {
    background-color: #4b8568;  /* dark green, same as link color */
  }

  .main-nav .active a {
    color: #eee;            /* light gray, same as navbar */
  }

  /* etc */
```

Note that: 

* We don't need a specialized "button" element for navigation: we're not submitting anything, we're following hyperlinks. 
* Instead, we can just style our `<a>` or `<li>` directly (or by adding classes directly to those elements), so it *looks and feels* like a button.
* This is a direct outcome of the Box Model you read about in the tutorial.

### When you're ready to work on appearances, test CSS rules directly in the browser

As some of you have discovered, the HTML previews you can get within VS Code are only really approximations of what you'd get in a real browser. So you probably want to get in the habit of having your file truly open in Firefox or Chrome.

Why those two browsers? Because they have great built-in developer tools to "inspect" elements of the page. It's already available: just **right-click anywhere and choose "inspect element"** to see the local html, the _full cascade of CSS rules_ that apply to it, and a few other features beside. 

<aside class="alert alert-info">Safari can do this, too, but you'll need to <a href="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html">activate it first</a>... and then "show the details sidebar."</aside>

This is helpful for a number of reasons: 

<ol>
  <li>First, to see how an existing site works. Viewing the full page source is great for seeing how professional designers organize their documents, but most of the time, you'll want to be more targeted: you don't _want_ to have to sift through everything just to figure out the color or font on that one blockquote or button (or whatever it is you want to imitate and thereby learn from). <strong>The inspector lets you zoom in on one html element</strong>, and leave everything else collapsed (until you want it).</li>

  <li>Second, any time you can't figure out why something's not working, the inspector is your best friend: it shows <em>what the browser thinks</em> you told it to do, rather than what you hoped you told it to do.</li>
  
  <li>Third, you can use the inspector to simulate a mobile device! Look for the phone symbol. 
    <figure>
      <img src="../assets/img/inspector-toolbar--firefox.png" alt="firefox inspector toolbar" />
      <figcaption>In Firefox, the button's on the right of the toolbar</figcaption>
    </figure>
    <figure>
      <figcaption>In Chrome, it's on the left</figcaption>
      <img src="../assets/img/inspector-toolbar--chrome.png" alt="chrome inspector toolbar has the mobile emulator on the left" /> 
    </figure>
  </li>

  <li>Crucially, you can also <em>add CSS rules</em> and immediately see what effect they would have on the page. (Safari users, note that the button to add a new rule is on the bottom left, not the top right as in the other two browsers.) Color pickers are an especially nice feature – and perhaps the one thing that Chrome's inspector does better than Firefox's at the moment, in that Chrome lets you change from hex color to RGBA or HSL, and directly adjust saturation / luminosity, e.g. to improve contrast.</li>
</ol>

<!-- <figure role="figure">
<img src="{{site.github_url}}/assets/img/inspect-element--firefox--skeleton.gif" alt="screencast of the firefox in-browser inspector" />
</figure> -->

<div class="alert alert-warning">
<p>Just be sure to <strong>copy your changes to a file for safe keeping</strong>, or they'll disappear when you refresh!</p> 

<p>To make copy/paste easier, click on the source your browser created for your new rules: in Firefox it's called "inline", in Chrome "inspector-stylesheet", in Safari "Inspector Stylesheet."</p>
</div>

<div class="alert alert-info">
I've recorded a <a href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=befd7ed1-81e0-4f73-a28e-afc7010eb105">brief screencast demonstration of these tools</a>, should you wish to see it at home.
</div>

## 2. Ideas for studio

In a moment, I'm going to invite you to set goals for studio time: if you've kept up to date with the tutorials, you should now know enough to really start coding your own content!

**If you haven't yet sorted out your navigation, that's a great place to start.**

Here are some other things to consider as you move forward:

<details><summary>The semantic html tutorial would be useful now, as well as later!</summary>
<p>I hadn't initially scheduled it at this point in the tutorial, in large part because the tutorial itself doesn't introduce semantic elements like <code>&lt;section&gt;</code> and <code>&lt;nav&gt;</code> until later. But you may well find them easier to use than <code>&lt;div&gt;</code>, <code>&lt;div&gt;</code>, <code>&lt;div&gt;</code> all the time!</p>
<p>It'll also set you up well for the <a href="https://docs.google.com/forms/d/e/1FAIpQLSfPzuLPbCkRQ7k4--R8Ti7zkM1zzLP-jlZ7MwQIShlyeiU6Kw/viewform">accessible HTML workshop</a> tomorrow!</p>
</details>

<details><summary>Your homepage should probably be called something like index.html</summary>
<p>I'm going to recommend that everyone use GitHub Pages to publish your sites unless you have a good reason not to. (And you might; but talk to me about it.) In that system, you store your files in a GitHub repository (in a branch called "gh-pages," like this site, or a subdirectory called "docs" – look in your own repos!), and GH knows where to look to find your stuff. <em>By default, it'll show your README.md file as the home page, unless it finds a file called index.html or index.md</em>.</p>
<p>Therefore, rather than call your landing page myproject.html, landing.html, or home.html, you're better off using the index.html name. You can always change the <code>&lt;title&gt;</code> to give it a more accurate name in the browser tab. : )</p>
</details>

<details><summary>Strive for semanticity.</summary>
<p>
Ask yourself:
<ul>
  <li>Can you tell what's going on just by reading the HTML file?</li>
  <li>Do your header levels (<code>&lt;h1&gt;, &lt;h2&gt;</code>, etc) correspond to your intended hierarchy? Don't skip levels.</li>
  <li>Does the HTML hard-code any display (e.g. <code>&lt;center&gt;</code>, <code>&lt;b&gt;</code>) that should be in the CSS? (Older tutorials will suggest this, but it's not a great idea.)</li>
</ul></p>
</details>  

<details>
  <summary>Let appearances reflect the structure, not vice-versa</summary>  <p>This one's related to what I said above, but applies especially when you're starting to think about appearances. <em>Visuals are volatile; structure should be steady.</em> It can be very tempting to just accept your browser's default styles as a given, e.g. to jump from a large <code>&lt;h1&gt;</code> page title to an <code>&lt;h5&gt;</code> subtitle because the latter "looks about right." But this would mis-represent the actual structure of the document – and would seriously confuse screen-reader software trying to present the page to a blind visitor. Instead, use your browser's Inspector to take note of the CSS rules defining that <code>&lt;h5&gt;</code>, and apply them to <code>&lt;h2&gt;</code> in your stylesheet.</p><!-- This makes a good jump-point into the inspector... -->
</details>

<details> <!-- CONSIDER: SHOULD WE DO THIS ALL TOGETHER? If so, today or next time?? -->
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

 In the [shared google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes), **set a goal for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project? Note that a Website Preview is due a week from today.

<div class="alert alert-info">
If you haven't yet, please do expand and read my notes above. Also remember that you have many <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website; for today, might I especially point out the <strong>design advantages of <a href="https://loremipsum.io">placeholder text</a> and/or <a href="https://loremipsum.io/21-of-the-best-placeholder-image-generators/">images</a></strong>?
</div>



Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

<strong>Reply to your note in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">google doc</a>.</strong>
</div>

# Homework for next time
* **View** Kevin Powell's video on [5 simple tips to making responsive layouts the easy way](https://www.youtube.com/watch?v=VQraviuwbzU&list=PL4-IK0AVhVjM6kuUoUexfmnD8vHtZkXdd&index=4). It's also just a really useful channel to know about!
* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), including at least Flexbox (8) and Responsive Design (10), if you haven't yet.
  - As a reminder, you should **write out the exercises in the tutorials** and push them to your repository – probably in the tutorials subfolder. Once you have them working as presented, feel free to update them to test out ideas for your own site! But do try to confirm you can get them working first. HTML, like all code, is fiddly: punctuation (including spaces) matters for things like close-tags and CSS selectors.
* Separately, also **read** about [Grid Layout](https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725) (and optionally the followup post on [responsive grid](https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f)).
  - EXT: Want more CSS Grid templates and examples, including CodePens to play with? Try [Grid By Example](https://gridbyexample.com/patterns/, which also has video tutorials.
* **Compose and push** a first website preview: a beginning, focused on content and navigation.
