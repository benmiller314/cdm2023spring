
# Web Unit Workshop

**Work to have done**: a solid attempt at a complete website, ideally meeting baseline criteria. Rough edges are still welcome.

**Plan for the day**:

<div class="alert alert-danger">
<p>As a reminder, this lesson plan is fully asynchronous to allow you the maximum flexibility for vaccinations, midterms, and self-care.</p>

<p>To enable your partners to make use of your feedback in the upcoming synchronous studio, <strong>please post your responses to their GitHub repos by Thursday morning if at all possible.</strong> Thank you!</p>
</div>

1. Identify your partners
2. Work through the workshop cycle (3 times 15-20 min)
  - Describe what you see
  - Evaluate using our shared criteria
  - Suggest ways to level up
  - Post comments on the latest commit
3. Repeat (and reflect)
4. EXT homework: forum on consolidation unit

## 1. Identify your partners
As usual, you'll want to click through to the next three people in your row, wrapping around when you hit the end.

<div class="alert alert-info">
NB: If one of your partners has not yet posted a draft, contact them to ask about it (you can reply to one of my emails), and try (if you can) to loop back later this week: we're all trying to accommodate Flex@Pitt the best we can.
</div>

* <a href='https://github.com/gregsexauer/website-portfolio-2021spring'>Greg</a>, <a href='https://github.com/cmgo412/website-portfolio-2021spring'>Caela</a>, <a href='https://github.com/TBrusilovsky/website-portfolio-2021spring'>Thomas</a>, <a href='https://github.com/cap-alt-delete/website-portfolio-2021spring'>Carolyn</a>, <a href='https://github.com/boredhero/website-portfolio-2021spring'>Noah</a>
* <a href='https://github.com/hua-tori/website-portfolio-2021spring'>Tori</a>, <a href='https://github.com/patrickjmeyer/website-portfolio-2021spring'>Patrick</a>, <a href='https://github.com/Gley21/website-portfolio-2021spring'>Garrett</a>, <a href='https://github.com/aer84/website-portfolio-2021spring'>Abby</a>, <a href='https://github.com/gdelallo/website-portfolio-2021spring'>Grace D</a>
* <a href='https://github.com/gmh32/website-portfolio-2021spring'>Grace H</a>, <a href='https://github.com/annaruz/website-portfolio-2021spring'>Anna</a>, <a href='https://github.com/rmanyeka/website-portfolio-2021spring'>Rutendo</a>, <a href='https://github.com/TrentFoster/website-portfolio-2021spring'>Trent</a>, <a href='https://github.com/jackie216/website-portfolio-2021spring'>Jackie</a>
* <a href='https://github.com/paytonareed/website-portfolio-2021spring'>Payton</a>, <a href='https://github.com/anatems1/website-portfolio-2021spring'>Mason</a>, <a href='https://github.com/kle39/website-portfolio-2021spring'>Kenzie</a>, <a href='https://github.com/young1m030/website-portfolio-2021spring'>Maggie</a>, <a href='https://github.com/reaial/website-portfolio-2021spring'>Reaia</a>


Go ahead and click through to your partners' repos, and **download the zip file** by clicking on the green <img class="d-inline-block" src="../assets/img/github-code-btn.png" alt="code" /> button. It'll be a faster download than cloning, with just the latest snapshot. (But if you want to see revision history, you'll have to do it on the web.)

<details><summary>Show me</summary>
<figure role="figure"><img src="../assets/img/github--clone-code-zip.png" alt="Code button to clone repo; also includes the URL to use with the command line." /></figure>
</details>

<div class="alert alert-info">
<p>To make this process easier, you should probably indicate in your README.md file where to find the main files for your own project: what folder are they in, if not the docs folder?</p>

<p>Relatedly, if you're using Jekyll or React or something like it, please give instructions on how to load your most current rendered website, e.g. a link to the published GitHub Pages site. In that case, partners, you may want to View Source on the final rendered page.</p>
</div>


## 2. Work through the workshop cycle

Like the last two times, I'd like you to use a workflow that, first and foremost, *helps you see what's already happening.*  

It takes practice! Please do try: it helps make your comments more concrete and actionable, for both your partner and yourself. It's great to like something, but _if you can't say **what** you liked, the creator can't build on that knowledge as effectively... and **you** may not be learning as much as you could by naming what you value._

**A good test is whether you can tell, just from reading your comment, what you were reacting to.**

<div class="alert alert-warning">Note for async workshop: You may want to time yourself. In class we wouldn't have more than 15-20 minutes for each of three partners.
</div>

### 2a. Describe what you see
Begin by saying back what's there, so your partner knows whether their intentions are being understood. NB: For this unit, in which display is a separate – and often challenging – concern, I'm going to ask you to use a <em>two-step description</em>:

* **First look at the HTML, and say back what you see there.** What seem to be the major content areas? What's given top-level focus? (e.g. what kind of things are getting their own pages, or what's at &lt;h1&gt; status within a page?) What's next in the hierarchy?
* Once you've done that, **turn to the browser and repeat the process for the display.** What's given visual weight? What falls "above the fold"? Where are you invited to go next?

### 2b. Evaluate using our shared criteria

Review the [baseline criteria and aspirational goals](http://bit.ly/cdm2021spring-notes#heading=h.9ab0yoso6slh) we set last week, which I'll paste below for convenience.

* Is your partner's draft meeting baseline criteria? If not, where not?
* Where is your partner's draft going beyond baseline? Is the draft already meeting any particular aspirations?
* Does the hierarchy of the display correspond to the hierarchy implied by the HTML? If not, describe where they differ.

NB: This is still a form of description, not a judgment of anyone's ability. We're all still learning here!

<details><summary>Baseline</summary>
For a minimum grade of B, all projects for this unit must…
<ul><li>Use arrangement, size, color, visual rhythm, and/or contrast to focus viewers' attention.</li>
<li>Include at least 2-3 navigable html locations (multiple pages, or multiple scrolling locations on the same page)</li>
<li>Have a clear mode of navigation among the pages (no dead ends)</li>
<li>Include a sitewide css stylesheet (i.e. an organized visual theme)</li>
<li>Include at least one legally useable image, with alt text</li>
<li>Successfully display locally in a web browser</li>
<li>For all of the above, argue in the reflection why you did what you did – or what you would do if you had more time</li>
<li>Use meaningful commit messages that say what’s changing (or even why)</li></ul>
</details>

<details><summary>Aspirational</summary>
<p>To target (but not guarantee) a grade above a B, the best projects for this unit may do some (but probably not all!) of the following:</p>

<em>Media Files</em>
<ul><li>Include playable media: <code>&lt;audio&gt;</code>,  <code>&lt;video&gt;</code>, <code>&lt;iframe&gt;</code>)</li>
<li>Use many images, laid out in a clear pattern (e.g. grid, alternating left/right)</li>
<li>Optimize image filetypes, resolutions, and file sizes for faster loading</li>
<li>Make or modify your own multimedia content (e.g. graphics, audio, video)</li>
<li>Have a system to display other sorts of media files from the browser (docs, pdfs, etc)</li></ul>

<em>Dynamism</em>
<ul><li>Use responsive design (e.g. <code>@media</code> queries, <code>flex-wrap</code>, <code>auto-fill</code>, etc) to dynamically resize elements based on viewport width</li>
<li>Animate HTML elements via JavaScript (e.g. image carousel) or CSS (e.g. <code>:hover</code> / <code>:focus</code> events)</li>
<li>Add interactivity via JavaScript (e.g. on-click events) or other ways to receive information from site visitors (e.g. mailto: links, forms)</li>
<li>Include a loadable alternate stylesheet / theme (e.g. dark mode, high-contrast) if you can explain why it’s helpful in your reflection (e.g. does it make the site more accessible? Is it a print stylesheet?)</li>
</ul>

<em>Coding</em>
<ul><li>Use Flexbox or Grid (or Float) layouts</li>
<li>Use advanced navigation, e.g. drop-down menu, tabs, or sticky nav bar</li>
<li>Condense your CSS stylesheet to the best of your ability</li>
<li>Use Jekyll to minimize repetition in your HTML through templates and variables</li>
<li>Use a web framework to build your website (angular, react, etc. but also bootstrap, skeleton, etc, depending on your level)</li>
<li>Use JavaScript for anything at all</li>
<li>Add comments, whitespace, and other formatting to code to make it more readable</li>
</ul>

<em>Audience Engagement</em>
<ul><li>Use best practices for accessible design (see W3's Four Principles and the WAVE web accessibility evaluation tool)</li>
<li>Design for mobile devices (e.g. with <code>@media</code>)</li>
<li>Load site publicly over the internet (e.g. with GitHub Pages)</li>
<li>Have a clear, consistent theme for your website’s content</li>
<li>Apply visual unit knowledge about fonts and how they convey which message or how certain fonts pair together</li>
</ul>

<em>Reflection</em>
<ul>
<li>Make a clear argument in your reflection as to why you met enough of the aspirational criteria to be stretching the abilities you came in with</li>
<li>Justify the website's structure for its intended purpose / audience</li>
<li>(For all of the above, argue in the reflection why you did what you did – or what you would do if you had more time)</li>
</ul>
</details>

### 2c. Suggest ways to level up

* Is the draft almost meeting any particular aspirational goals? Which would you suggest trying next?
* Any other ways to improve that you can suggest, based on the readings and advice we've discussed in this class?
* If there was a mismatch between the hierarchies in the presentation and the content, which would you suggest changing, given what you think the intention was? (And here's where revision histories may be helpful, if you have time.)

### 2d. Post comments on the latest commit
Finally, make sure you **post** all these comments – in language you'd be comfortable sharing publicly – on the latest commit on the project's GitHub website.

As a reminder, here's how and where to leave comments on GitHub: Just...

* click through to the history of commits (the clock button);
* click on the _commit hash_, the set of random-seeming numbers and letters almost at the end of the top row (i.e., for the most recent commit); and
* scroll to the bottom of the _diff view_ that appears. You'll see a comment box there: <figure role="figure"><img src="../assets/img/github--comment-on-commit.gif" alt="screencast of the three steps just described"/></figure>


## 3. Repeat (and reflect)
Repeat the steps above for your next two partners' repos. On subsequent loops, note that **after** viewing the project first, you may also want to read and/or refer to the previous comments.

But this is not just a way of ensuring that you get feedback from three partners; **workshop is also a way of training your eyes, and of realizing new possibilities.** As we head into Thursday's studio class, think about what you've seen that _you'd_ like to try. What suggestions would you give yourself, now that you've given suggestions to others?


<div class="alert alert-warning">
I said above that peer reviews are due ideally by Thursday morning; even if that's not possible, please be sure to have them completed no later than Thursday at 2:30pm, so your partners have them for in-class studio.
</div>

## EXT: Thinking ahead
* As I did at the same point in the audio and visual units, I'm inviting you to think forward into the final unit, when you'll work to consolidate or build on what you've learned – possibly in partnership with your peers. See <a href="{{site.github.issues_url}}">the issue queue</a> for more details.
* There is no minimum length for this post, but I am interested to see if you're still thinking about working as a large group on a collective book or canvas project...
