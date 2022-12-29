
# Web Unit Post-Workshop Studio

**Work to have done**: asynchronous peer-review; optional [forum post about possible consolidation-unit projects]({{site.github.issues_url}}/13)

**Plan for the day**:

* Back to the feedback
* Planting seeds
* Gathering questions
* Studio time
  - set an intention
  - work time
  - exit note


## Back to the feedback

I had set the deadline for asynchronous workshop fairly close to the start of class, so as of my writing this, a lot of notes were still missing. Please **open up your website repo, head into the history, and see if you have any unread comments there.**

Hopefully everyone has by now received at least 2 (ideally 3) comments from members of your workshop groups! **If you have not, please let me know**, so I can make sure you've got a diverse set of perspectives on your work in progress.

## Planting seeds

As a reminder, here's my [general advice already given](lesson-18):
* Call your homepage index.html
* Strive for semanticity
* Let appearances (CSS) reflect the structure (HTML), not vice-versa
* Be sure to include some [basic spacing](http://jgthms.com/web-design-in-4-minutes)

In addition, I hope you can...

<details>
<summary>Remember to update your README.</summary>
It should have a brief description of the project, and may I also suggest an active link to your live website, if you have one?
</details>


<details><summary>Level up line breaks into space between paragraphs.</summary>

<p>The <code>&lt;br/&gt;</code> tag is not really for spacing, but rather for creating manual line breaks. Think poetry, or maybe a two-part heading where you want to enforce a particular phrasing (e.g. a line break after a colon). The line break should itself be meaningful.</p>

<p>So instead of adding a <code>&lt;br/&gt;</code> after your paragraphs, give the paragraphs some <code>margin-bottom</code>; 1em or slightly more (depending on your <code>line-height</code>) should do the trick.</p>

<!-- put a gif here of adding and removing margin -->
</details>

<details><summary>Level up your ordered lists.</summary>

Did you know you can choose the number an <code>&lt;ol&gt;</code> list starts with?

You can also <a href="https://css-tricks.com/almanac/properties/l/list-style">choose different list-item-types</a> for alphabetical or roman counting systems. Same goes for bullets in your <code>&lt;ul&gt;</code>'s.
<figure role="figure">
<p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="matt-west" data-slug-hash="DCEzd" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="HTML List Demos">
  <span>See the Pen <a href="https://codepen.io/matt-west/pen/DCEzd">
  HTML List Demos</a> by Matt West (<a href="https://codepen.io/matt-west">@matt-west</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>
</figure>

</details>

<details>
<summary>Articulate permissions.</summary>

<p>If you're using resources you didn't make yourself, be sure to include enough information to recover where it came from: a direct link to the image and to the specific license (if there is one) is ideal. Creative Commons sources often provide that html for you!</p>

<p>Where to put this information? Ideally, somewhere small near the image itself. (There's a semantic html way of doing this with <code>&lt;figure&gt;</code> and <figure role="figure">&lt;figcaption&gt;</figure>, which you may remember from <a href="https://www.internetingishard.com/html-and-css/semantic-html/#figures-and-captions">the Semantic HTML</a> section of the tutorial. See also <a href="https://www.scottohara.me/blog/2019/01/21/how-do-you-figure.html">this extended discussion of figures, figcaptions, and alt text</a>.)</p>

<p>Alternately, you can have a rights page somewhere, or use the site footer – or have a live hyperlink from your site to an external credits.md file in your repo.</p>

<div class="alert alert-info"><em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See the homework reading after <a href="lesson-04">Lesson 4</a> to review the Four Factors you need to consider.</div>
</details>

<!-- <details>
<summary>Call your homepage index.html (or index.md)</summary>
By default, this is what a web browser will display when you just type in the URL of your website: it is, in other words, the default filename for your home page. If your home page currently has another filename, <a href="https://www.lifewire.com/index-html-page-3466505">you probably want to change it to index.html</a>. You can always keep your more interesting name as the &lt;title&gt;!
</details> -->

<details>
<summary>Have alt text for all your images.</summary>
<p>Text-alternatives, which you add to images using <code>&lt;img alt="text description here" src="path/to/source.jpg"&gt;</code>, are a required element in validated html. They're also really helpful, and not only to blind users: they make the html file more readable on its own, and thus more semantic, and they help you troubleshoot layout when image paths are broken by showing you where each image is trying to appear.</p>

<p>For more guidance on how to write useful alt text, see <a href="https://webaim.org/techniques/alttext/">https://webaim.org/techniques/alttext/</a>.</p>
</details>

<!-- <details>
<summary>Consider titles.</summary>

A title can provide a context, a clue, a genre, a commentary; it can add an extra layer to viewer expectations. In previous units, you were titling your entire project; for a website, every page has its own <code>&lt;title&gt;</code> element in the <code>&lt;head&gt;</code>, which will show up in the browser's tab. These titles <em>could</em> be the same for all your pages, but they could also vary. What text do you want on top of the window, to show users where they are?
</details> -->



<details>
<summary>When revising, take the lowest line-count challenge.</summary>

<p>This is primarily a polishing step after all your content and style is pretty much set – but it may also help you clarify what your HTML is really doing, which can in turn make it easier to style.</p>

<p>Do your CSS rules repeat each other? Maybe they can be combined. <ul>
  <li>Look for elements that all behave the same way, and give them a shared class.</li>
  <li>Remember that you can apply more than one class to the same html element, so you can make rules for shared attributes in one class and special cases in another.</li>
</ul></p>

<p>Does your HTML have lots of containers with only one element in them?
<ul>
  <li>Some containers are important for positioning, e.g. centering with a flexbox.</li>
  <li>Others, though, are unnecessary clutter: if you can "unwrap" the element and apply CSS rules directly to it, with no loss in function, go ahead and unwrap it. You can usually move classes from an outer element straight onto the inner one. See my <a href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9171fa85-be27-437d-99b9-acfa00f44a4f">demo video from last week</a> for an example.</li>
</ul></p>
</details>


## Gathering questions

As you finish taking in the advice of your peers (and going over my suggestions above), I'd like to know **what questions you have that I might be able to help with** – especially if it's about something you've seen in assigned readings or revision suggestions, but you're not sure how to implement.

<div class="alert alert-success">
Head into <a href="http://bit.ly/cdm2021spring-notes">the google doc</a> and write down what you're thinking about. It can be anonymous!</div>

I'll work through these in the Q&A room, and record my responses when they're ready, to post on Canvas. But if you're posting a question you'd like direct help with, please come on in! I'll start with those live questions.

## Studio Time!

### Set an intention
As usual, before you start, <a href="http://bit.ly/cdm2021spring-notes">go to the next section of the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
  <ul>
    <li>Work on responsive layout?</li>
    <li>Work on replacing placeholder content with real content?</li>
    <li>Work on streamlining your code?</li>
    <li>Work on one of your stretch goals?</li>
    <li>etc etc</li>
  </ul>
Just a sentence or two as a guidepost will give you something to come back to, to reorient, if you find yourself walking in circles or caught in a thicket.

<div class="alert alert-warning">
Don't forget to save periodically as you go:
 <ul>
   <li>as an html / css / js file</li>
   <li>as a git commit, saying what you've just achieved</li>
   <li>as a screenshot</li>
 </ul>
</div>

### Work Time
Please ask questions as they come up. Otherwise, I'll try to work through the questions from the doc.

### Exit Note
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular CSS skill? Decide something about your project? Raise a question in a new way that you'd like some help with?


# Homework for next time

* Aiming for 11:59pm on Sunday, **complete – at least for now – your website.** Your repository (on GitHub or in a shared Box folder) should include:
   - A multifile **project folder** (probably called "docs"), containing a combination of html and css files
   - At least one more static **<a href="https://www.take-a-screenshot.org/">screenshot</a> (.png or .jpg)** of your web pages in progress.
     * Think about what moments are worth remembering as you go: where did you level up, or realize something, or get stuck?
   - An **updated README.md file**, introducing the Website source code to a new audience.
   - An updated ASSETS.md (or CREDITS.md) file reflecting what you actually used, including documentation of any outside sources and your permission to use them (e.g. explicit licenses like CC, or rationales for claiming fair use)
      * If you want, this can be a live page (or a footer) on your website.
   - An updated README.md file introducing your website to a new audience. Make it something to live beyond this assignment, if you can. :¬)
* **By 11:59pm on Tuesday, write a prose reflection** that incorporates images from your feedback and screenshots of your Atom project and the website itself. As explained in the [prompt for the assignment](https://github.com/benmiller314/website-portfolio-2021spring#project-3-website-portfolio), this should include:
   - At least 500 words
   - Your own assessment of how you met the baseline criteria and goals for the unit, as well as any aspirational criteria as appropriate
   - At least one photograph of feedback you used to revise (and please say how)
   - At least one or two screenshots of your work in progress (ideally, related to the discussion in the previous two bullets)
* **Post your reflection** to the course site's [Issue queue]({{site.github.issues_url}}), to make it easier to embed images.
   - If you want to then copy the source code into a file in your repo called reflections.md, I won't stop you!
   - If you feel strongly that you'd rather keep your reflection private, you can email it to me instead. But my default assumption is that we learn from each other as much as from ourselves, so I hope you can find a way to write publicly about your experience with this project.
