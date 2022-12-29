---
layout: bottomnav
---

# Web Unit Studio / Deployment

**Work to have done**:

* As much of the [Interneting is Hard (but it doesn't have to be)](http://web.archive.org/web/20190213013947/https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors")
* A website proposal, posted to the [Issue Queue]({{site.github.issues_url}}/)
* More reading on [CSS selectors](https://css-tricks.com/how-css-selectors-work/) and [GitHub Pages](https://pages.github.com/)

**Plan for the day**:

1. Web Design in 4 minutes (in 15 minutes)
2. Ben's takeaway: a suggested composing strategy
3. Go forth!
4. Exit note


## 1. Web Design in 4 minutes (in 15 minutes)

Designer Jeremy Thomas created a nifty little walkthrough for how to think about building up a stylesheet, which you can find at [jgthms.com/web-design-in-4-minutes/](http://jgthms.com/web-design-in-4-minutes/). Now that you're more familiar with CSS rules and selectors, I want to talk through it together, _as a way of modeling how you might spend your work-time in studio today_ and over the next week or so.

### 2. Ben's take-away
<details>
<summary>a suggested composing strategy</summary>
<ol>
   <li>List out your content sections</li>
   <li>Decide what's nested, what's at the same level</li>
   <li>Draw boxes, and label them<!-- SKIPPABLE --></li>
   <li>Use the boxes<!-- list/nesting --> to write HTML containers<!-- ELEMENTS: only div if you have to --></li>
   <li>Use the labels to give them CSS classes</li>
   <li>Only then start to style the classes</li>
   <li>Use some standard minimum styling
      <ul>
         <li>set a maximum width for text</li>
         <li>give your main content and headers some padding</li>
         <li>change font default away from "Times"</li>
      </ul>
   </li>
</ol>
</details>

<!-- FOR NEXT TIME
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
<strong>Important</strong>: if you don't yet know how to deploy a project site using GitHub pages, <a href="https://help.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site">learn how before you leave today</a>. It's not hard, and you don't need to create a new repository! Just <ol>
<li>create a folder in your repo called "docs,"</li>
<li>put your website's files in there, and </li>
<li>change the settings for the repo to "use master branch /docs folder" as your source.</li>
</ol>
Then your site will build at https://<em>your-username</em>.github.io/<em>your-repo</em>. There are more options you can read about, but that's it in a nutshell!

If you're worried about showing up in search results before your site is ready, you can always <a href="https://support.google.com/webmasters/answer/93710">add a noindex meta tag</a>.
</div>

<div class="alert alert-info">
Remember that you have <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website. For today, might I especially point out the design advantages of <a href="https://loremipsum.io">placeholder text</a>?
</div>

Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

**Write me a quick email.**

# Homework for next time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), including at least Flexbox (8) and Responsive Design (10), if you haven't yet.
* **Compose and push** a website preview: a beginning. As detailed in the assignment, this should include:
<ul><li>A multifile <strong>project folder</strong> (probably named "docs," for ease of use with GitHub Pages), containing a combination of html and css and image assets, even if the whole thing is not yet well-developed.</li><li> A static <strong><a href="https://www.take-a-screenshot.org/">screenshot</a> (.png or .jpg)</strong> of your website-in-progress, as rendered in a local web browser (for comparison later to subsequent drafts). <ul><li>(Optionally, take a screenshot of your Atom project setup, too.)</li></ul></li><li> A plain text (.txt) or markdown (.md) file, explaining in at least 300 words <strong>what you're showing us</strong> in this preview. Feel free also to ask questions or lay out next steps for yourself!</li><li> An updated <strong>ASSETS.md</strong> file, now with any files or fonts you've actually obtained. As you go, add source documentation for any outside sources – and your permission to use them (e.g. licenses, fair use; see <em>Writer/Designer</em> p. 160-165).</li></ul>
