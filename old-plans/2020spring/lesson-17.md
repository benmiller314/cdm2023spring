---
layout: bottomnav
---

# Web Unit Studio / Deployment

**Work to have done**:

* As much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors")
* More reading on [CSS selectors](https://css-tricks.com/how-css-selectors-work/)
* A website proposal, posted to the [Issue Queue]({{site.github.issues_url}}/)


**Plan for the day**:
1. General responses / advice on proposals
2. Go forth!
3. Exit note


## 1. General responses / advice on proposals

<details>
<summary>Start by thinking about structure</summary>

<p>Remember from last time that though you probably have a vision for how your site should <em>look</em>, it makes sense to <strong>begin by thinking about the <em>structure of your content</em></strong>. That will give you the material you need to support <em>multiple</em> views, depending on screen size and/or what begins to feel most important.</p>

<p>So I recommend starting by listing and grouping:
<ol>
  <li>What are the content sections your site will include?</li>
  <li>How might you group those things hierarchically? That is, what's the most important for a viewer to encounter first? Which things are (or could be) parts of others, and which things have to be at the same level?</li>
  <li>If you can make a nested list of your content areas, that could serve you as a navigation... and probably also a list of headers (<code>&lt;h1&gt;</code>, <code>&lt;h2&gt;</code>, etc).</li>
</ol>
</p>
</details>

<details>
<summary>Beware of scope creep; plan for phased releases</summary>

<p>Bear in mind that you only have a couple more weeks on this project. If you've just given yourself an ambitious agenda, think about "minimum deliverable product" and "stretch goals." You have version control; you can iterate. In other words: you can always come back and add <em>more</em>, but it's good to start with what's really at the <em>core</em> of your website idea.</p>

</details>

<details>
<summary>Use the structure to guide appearance, not vice-versa</summary>
<p>This one's related to the first, but applies when you're starting to think about appearances. <em>Visuals are volatile; structure should be steady.</em> It can be very tempting to just accept your browser's default styles as a given, e.g. to jump from a large <code>&lt;h1&gt;</code> page title to an <code>&lt;h5&gt;</code> subtitle because it "looks about right." But this would mis-represent the actual structure of the document – and would seriously confuse screen-reader software trying to summarize the page for a blind visitor. Instead, take note of the CSS rules defining that <code>&lt;h5&gt;</code>, and apply them to <code>&lt;h2&gt;</code> in your stylesheet.</p>
</details>

<details>
<summary>Take advantage of classes to limit the scope of CSS rules</summary>
<p>If you're worried they'll carry too broadly, affecting inner page <code>&lt;h2&gt;</code>'s when you only meant it to apply on the front page, just limit the scope of the css rule. The following code will only apply to <code>&lt;h2&gt;</code>'s inside a <code>&lt;body class="front"&gt;</code>:
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

This has the extra advantage that you can set a lot of other rules for <em>all</em> <code>&lt;h2&gt;</code>'s, and just add the tweaks you need for the subtitle in this additional ruleset.
</p>
</details>

<details>
<summary>When you're ready to work on appearances, test CSS rules directly in the browser</summary>

<p>Chrome and especially Firefox have great built-in developer tools to "inspect" elements of the page. It's already available: just right-click anywhere and choose "inspect element" to see the local html, the full cascade of CSS rules that apply to it, and a few other features beside. (Safari can do this, too, but you'll need to <a href="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html">activate it first</a>... and then "show the details sidebar.")</p>

<p>Crucially, you can also <em>add CSS rules</em> and immediately see what effect they would have on the page. Color pickers are an especially nice feature. (Safari users, note that the button to add a new rule is on the bottom left, not the top right as in the other two browsers.)

<figure>
<img src="../assets/img/inspect-element--firefox--skeleton.gif" alt="screencast of the firefox in-browser inspector" />
</figure>

Just be sure to <strong>copy your changes to a file for safe keeping</strong>, or they'll disappear when you refresh! To make copy/paste easier, click on the source your browser created for your new rules: in Firefox it's called "inline", in Chrome "inspector-stylesheet", in Safari "Inspector Stylesheet."
</p>
</details>

<details>
<summary>Stuck for what to do, CSS-wise? Start with some basic spacing</summary>

<p>This is what I was talking through last time: try rules from <a href="http://jgthms.com/web-design-in-4-minutes">Web Design in 4 Minutes</a>, like... <ul><li>set a maximum width for text</li><li>add padding on main content and headers</li><li>change font-family away from the default "Times"</li></ul></p>

</details>


<!-- FOR NEXT TIME, not today
## 2. Other notes

* Your homepage should probably be called something like index.html (or index.md) for it to load automatically at the root directory of your website URL. If you're getting a 404 error, that might be the reason.

* Take on the lowest line-count challenge. Ask yourself:
  - does that div need to be there?
  - could those CSS rules be combined?

* Strive for semanticity. Ask yourself:
  - can you tell what's going on just by reading the HTML file?
  - does the HTML hard-code any display (e.g. `<center>`, `<b>`) that should be in the CSS?  
-->

## 3. Go forth!

Do what you need to do to level up on HTML and CSS in the direction of your specific project; a Website Preview is due Thursday.

<div class="alert alert-white">
<strong>Did you know?</strong> If you're building a website in GitHub (and you are), you can publish it for free, using GitHub Pages! You don't need to create a new repository: Just <ol>
<li>have a folder in your repo called "docs," [DONE]</li>
<li>put your website's files in there (subfolders are fine), and </li>
<li>change the settings for the repo to "use master branch /docs folder" as your source.</li>
</ol>
Then your site will build at https://<em>your-username</em>.github.io/<em>your-repo</em>. There are more options you can read about, but that's it in a nutshell!

If you're worried about showing up in search results before your site is ready, you can always <a href="https://support.google.com/webmasters/answer/93710">add a noindex meta tag</a>.
</div>

<div class="alert alert-info">
Remember that you have <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website. For today, might I especially point out the design advantages of <a href="https://loremipsum.io">placeholder text and/or images</a>, once you know what your main content areas and headers will be?
</div>


Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

<strong>Write me a quick email.</strong>
</div>

# Homework for next time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), including at least Flexbox (8) and Responsive Design (10), if you haven't yet.
* Separately, **also read** about [Grid Layout](https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725) on Medium (and optionally the followup post on [responsive grid](https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f)). Author Rafaela Ferro includes screencasts, and also pictures of cute dogs!
* **Compose and push** a website preview: a beginning. As detailed in the assignment, this should include:
<ul><li>A multifile <strong>project folder</strong> (probably named "docs," for ease of use with GitHub Pages), containing a combination of html and css and image assets, even if the whole thing is not yet well-developed.</li><li> A static <strong><a href="https://www.take-a-screenshot.org/">screenshot</a> (.png or .jpg)</strong> of your website-in-progress, as rendered in a local web browser (for comparison later to subsequent drafts). <ul><li>(Optionally, take a screenshot of your Atom project setup, too.)</li></ul></li><li> A plain text (.txt) or markdown (.md) file, explaining in at least 300 words <strong>what you're showing us</strong> in this preview. Feel free also to ask questions or lay out next steps for yourself!</li><li> An updated <strong>ASSETS.md</strong> file, now with any files or fonts you've actually obtained. As you go, add source documentation for any outside sources – and your permission to use them (e.g. licenses, fair use; see <em>Writer/Designer</em> p. 160-165).</li></ul>
