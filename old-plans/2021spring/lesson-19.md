
# Web Unit Studio / Deployment

**Work to have done** (by Tuesday, but with catch-up as needed):

* As much of the [Interneting is Hard](https://internetingishard.com/html-and-css/) [(but at least it's WebArchive crawled)](https://web.archive.org/web/20201105195453/https://www.internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors")
* More on CSS selectors: the [CSS Diner](https://flukeout.github.io/) game and/or [a CSS-Tricks roundup](https://css-tricks.com/how-css-selectors-work/)
* A website proposal, posted to the [Issue Queue]({{site.github.issues_url}}/)


**Plan for the day**:
1. Brief intro to GitHub Pages
2. Reminder of needful things from last time
3. Set goals and go forth!
4. Update your goals
5. HW: first preview due Tuesday

## 0. Warm-up conversation

What did you guys think of the CSS Diner?

## 1. Brief intro to GitHub Pages

### What it is
In addition to the wonderful things we've already used GitHub for, like forking, cloud storage, and peer comments on commits, GH also lets you make a fully functional basic website – open to the public and everything – for free. They call it GitHub Pages.

Here's how it works: you store your files in a GitHub repository (in a branch called "gh-pages," like I do for this site, or a subdirectory called "docs" – look in your own repos!), and GH knows where to find your stuff.

### How to do it

To activate GH Pages,
1. Go to your repository Settings
2. Scroll down to where it says "GitHub Pages"
3. Change the source from "none" to "master"
4. Change the folder from "/ (root)" to "/docs"
5. Click "save."

And that's it! The settings should now show you the URL where your rendered HTML will appear. If it doesn't, just wait and/or try again; sometimes it takes a minute or two to refresh.

<figure role="figure"><figcaption>Here’s a visual representation of those instructions.</figcaption> <img src="../assets/img/github--activate-gh-pages.gif" alt="screencast enacting the ordered list above">.</figure>

### Tips and tricks
<div class="alert alert-warning">
One important caveat: <em>By default, it'll show your README.md file as the home page, unless it finds a file called index.html or index.md</em>.
</div>

Therefore, rather than call your landing page myproject.html, landing.html, or home.html, you're better off if you **name your homepage _index.html_**. You can always change the <code>&lt;title&gt;</code> to give it a more accurate name in the browser tab. : )

In addition, you should be aware that GH Pages takes a little time to render your latest changes. For faster feedback on the changes you make, you'll want to **view the local file in your browser**, rather than always waiting for the live site to load.

Finally, if you're feeling confident about code and want to make it less repetitive, GH Pages comes with the Jekyll templating engine built in. Setup for local development with Jekyll is a little more involved (it requires the command line and Ruby), but the documentation is pretty good. You can read more about it, and find a series of relevant links, on our [Resources page](https://benmiller314.github.io/cdm2021spring/resources#web-frameworks:~:text=Jekyll%20step%2Dby%2Dstep), at the end of the section on [Web Frameworks](https://benmiller314.github.io/cdm2021spring/resources#web-frameworks).

### In conclusion
<div class="alert alert-success">
I'm going to recommend that everyone use GitHub Pages to publish your sites unless you have a good reason not to. (And you might! But talk to me about it.)
</div>



## 2. Reminder of needful things from last time

* Beware of scope creep; plan for phased releases.
* Start by thinking about structure (i.e. HTML before CSS).
* You don't have to reinvent the wheel.
* When you're ready to work on appearances, test CSS rules directly in the browser.
  - Be sure to **copy your changes to your text editor for safe keeping** (i.e. Atom, by default), **or they'll disappear when you refresh!**
  - To make copy/paste easier, click on the source your browser created for your new rules: in Firefox it's called "inline", in Chrome "inspector-stylesheet", in Safari "Inspector Stylesheet."

<!-- a series of screenshots here would be nice, wouldn't it? -->

If you want a refresher on what any of those things mean, you can find more detail in [Tuesday's lesson plan](lesson-18). I also had these pieces of general advice:

* Strive for semanticity.
* Let appearances reflect the structure, not vice-versa.
* If you're stuck for what to do, CSS-wise, start with some basic spacing.
  - <a href="http://jgthms.com/web-design-in-4-minutes">Web Design in 4 Minutes</a> suggests what some of those basics might be.
  - For more advanced layout (sidebars, columns, grids, etc), see the links in the homework assignment.



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

In the [shared google doc](http://bit.ly/cdm2021spring-notes), **set a goal for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project? Note that a Website Preview is due on Tuesday, but the Website Draft isn't due until a full week after that. (I'm suggesting that you work on getting some content into HTML by Tuesday, and a starter layout into place by Thursday, April 1st.)

<div class="alert alert-info">
If you haven't yet, please do expand and read the notes from last class. Also remember that you have many <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website; for today, might I especially point out the <strong>design advantages of <a href="https://loremipsum.io">placeholder text</a> and/or <a href="https://loremipsum.io/21-of-the-best-placeholder-image-generators/">images</a></strong>?
</div>


<div class="alert alert-warning">
As usual, to get credit for asynchronous participation, please add your intentions and exit notes to the google doc when you start and stop working – and aim to work for at least two 20-minute pomodoros. <!-- (In class, we had about 50 minutes of straight-up studio time.) --> It helps me if you flag this as a suggestion or comment, so I get an email alert, but you can also just send an update email to me directly. : )
</div>


Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet? Work through a tutorial or two (and which)?

<strong>Reply to your note in the <a href="http://bit.ly/cdm2021spring-notes">google doc</a>.</strong>
</div>

# Homework for next time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), including at least Flexbox (8) and Responsive Design (10), if you haven't yet. (Broken record reminder: you can skip Floats.)
  - As a reminder, you should **write out the exercises in the tutorials** and push them to your repository – probably in the tutorials subfolder. That helps me know where I can be more helpful, especially if things are starting to go sideways.
  - Once you have the tutorial sample code working as presented, by all means update the pages to test out ideas for your own site! But _do try to confirm you can get them working first._ HTML, like all code, is fiddly: punctuation (including spaces) matters for things like close-tags and CSS selectors.
  - It might help to keep the tutorial files as written in the tutorials subfolder of your repo, and then save the duplicated-and-modified versions in your docs folder.
* Separately, also **read about [Grid Layout](https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725)** (and optionally the followup post on [responsive grid](https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f)).
  - If you want to practice with this code, go for it! Just create a new folder in your tutorials subfolder.
  - EXT: Want more CSS Grid templates and examples, including CodePens to play with? Try [Grid By Example](https://gridbyexample.com/learn/), which also has video tutorials (in a charming British accent, if you find that sort of thing charming).
* **Compose and push** a first website preview: a beginning, focused on content and navigation.
