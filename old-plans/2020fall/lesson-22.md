
# Web Unit Workshop

**Work to have done**: a solid attempt at a complete website, ideally meeting baseline criteria. Rough edges are still welcome.

**Plan for the day**:

<div class="alert alert-danger">
As a reminder, this lesson plan is fully asynchronous to allow you the maximum flexibility for Election Day.

If you haven't yet voted, and you are able to do so, <strong>please vote!</strong> Text your friends, and encourage them to vote, too, if they haven't. Your voices are more important even than schoolwork.
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

* [Alexa](https://github.com/AlexaSpaventa/website-portfolio-2020fall), [Brian](https://github.com/briansostek/website-portfolio-2020fall), [Kyle Maxwell](https://github.com/KyleMaxwell1224/website-portfolio-2020fall), [Jagr](https://github.com/jeepy33/website-portfolio-2020fall)
* [Lydon](https://github.com/LLP37/website-portfolio-2020fall), [Leia](https://github.com/leiawerner/website-portfolio-2020fall), [Ben Schatz](https://github.com/bschatz17/website-portfolio-2020fall), [Lucas](https://github.com/LDib/website-portfolio-2020fall)
* [Carly](https://github.com/carlystanford/website-portfolio-2020fall), [Hunter](https://github.com/hjo6/website-portfolio-2020fall), [Trinity](https://github.com/trinitymccool/website-portfolio-2020fall),  [Kevin](https://github.com/kevdliedel/website-portfolio-2020fall), [Nicholas](https://github.com/peekssezin/website-portfolio-2020fall)
* [Kyle O'Malley](https://github.com/jkomalley/website-portfolio-2020fall), [Christianna](https://github.com/csk32/website-portfolio-2020fall),  [Shreya](https://github.com/shreyababu/website-portfolio-2020fall), [Henry](https://github.com/heh44/website-portfolio-2020fall),
[Maia](https://github.com/Maials268/website-portfolio-2020fall)


Go ahead and click through to your partners' repos, and **download the zip file** by clicking on the green <img class="d-inline-block" src="../assets/img/github-code-btn.png" alt="code" /> button. It'll be a faster download than cloning, with just the latest snapshot. (But if you want to see revision history, you'll have to do it on the web.)

<details><summary>Show me</summary>
<img src="../assets/img/github--clone-code.png" alt="Code button follows 'go to file' and 'add file' options. 'Download zip' is the last option in the submenu the button brings up." />
</details>

<div class="alert alert-info">
To make this process easier, you should probably indicate in your README.md file where to find the main files for your own project: what folder are they in, if not the docs folder?

Relatedly, if you're using Jekyll or React or something like it, please give instructions on how to load your most current rendered website, e.g. a link to the published GitHub Pages site. Your partners will probably want to View Source on the final rendered page.
</div>


## 2. Work through the workshop cycle

Like the last two times, I'd like you to use a workflow that, first and foremost, *helps you see what's already happening.*  

It takes practice! Please do try: it helps make your comments more concrete and actionable, for both your partner and yourself. It's great to like something, but if you can't say *what* you liked, the creator can't build on that knowledge as effectively... and *you* may not be learning as much as you could by naming what you value.

A good test is whether you can tell, just from your comment, what you were reacting to.

<div class="alert alert-warning">You may want to time yourself: in class we wouldn't have more than 15-20 minutes for each of three partners.
</div>

### 2a. Describe what you see
Begin by saying back what's there, so your partner knows whether their intentions are being understood. NB: For this unit, in which display is a separate – and often challenging – concern, I'm going to ask you to use a <em>two-step description</em>:

* **First look at the HTML, and say back what you see there.** What seem to be the major content areas? What's given top-level focus? (e.g. what kind of things are getting their own pages, or what's at &lt;h1&gt; status within a page?) What's next in the hierarchy?
* Once you've done that, **turn to the browser and repeat the process for the display.** What's given visual weight? What falls "above the fold"? Where are you invited to go next?

### 2b. Evaluate using our shared criteria

Review the [baseline criteria and aspirational goals](http://bit.ly/cdm2020fall-notes#heading=h.80axmrlhvinn) we set last week, which I'll paste below for convenience.
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
<li>For all of the above, argue in the reflection why you did what you did – or what you would do if you had more time</li></ul>
</details>

<details><summary>Aspirational</summary>
To target (but not guarantee) a grade above a B, the best projects for this unit may do some (but probably not all!) of the following:

<em>Media Files</em>
<ul><li>Include playable media (music, video)</li>
<li>Use many images, laid out in a clear pattern (e.g. grid, alternating left/right)</li>
<li>Optimize image filetypes, resolutions, and file sizes for faster loading</li>
<li>Make or modify your own graphics using GIMP, etc</li></ul>

<em>Dynamism</em>
<ul><li>Use responsive design (e.g. <code>@media</code> queries) to dynamically resize elements based on viewport width</li>
<li>Animate HTML elements via JavaScript (e.g. image carousel) or CSS (e.g. <code>:hover</code> / <code>:focus</code> events)</li>
<li>Add interactivity via JavaScript (e.g. on-click events) or other ways to receive information from site visitors (e.g. mailto: links, forms)</li>
<li>Include a loadable alternate stylesheet / theme (e.g. dark mode, high-contrast) if you can explain why it’s helpful in your reflection (e.g. does it make the site more accessible? Is it a print stylesheet?)</li>
</ul>

<em>Coding</em>
<ul><li>Use Flexbox or Grid layouts
Use advanced navigation, e.g. drop-down menu, tabs, or sticky nav bar</li>
<li>Condense your CSS stylesheet to the best of your ability</li>
<li>Use Jekyll to minimize repetition in your HTML through templates and variables
Utilize a web framework to build your website (angular, react, etc. but also bootstrap, skeleton, etc, depending on your level)</li>
</ul>

<em>Audience Engagement</em>
<ul><li>Use best practices for accessible design (see W3's Four Principles and the WAVE web accessibility evaluation tool)</li>
<li>Load site publicly over the internet (e.g. with GitHub Pages)</li>
<li>Have a clear, consistent theme for your website’s content</li>
</ul>

<em>Reflection</em>
<ul><li>Use meaningful commit messages that say what’s changing (or even why), especially if that’s new to you</li>
<li>Make a clear argument in your reflection as to why you met enough of the aspirational criteria to be stretching the abilities you came in with</li>
</ul>
</details>

### 2c. Suggest ways to level up

* Is the draft almost meeting any particular aspirational goals? Which would you suggest trying next?
* Any other ways to improve that you can suggest, based on the readings and advice we've discussed in this class?
* If there was a mismatch between the hierarchies in the presentation and the content, which would you suggest changing, given what you think the intention was? (And here's where revision histories may be helpful, if you have time.)

### 2d. Post comments on the latest commit
Finally, make sure you **post** all these comments – in language you'd be comfortable sharing publicly – on the latest commit on the project's GitHub website.

Here's how and where to leave comments on GitHub: Just...

* click through to the history of commits (the clock page);
* click on the _commit hash_, the set of random-seeming numbers and letters almost at the end of the top row (i.e., for the most recent commit); and
* scroll to the bottom of the _diff view_ that appears. You'll see a comment box there: <figure><img src="../assets/img/github--comment-on-commit.gif" alt="screencast of the three steps just described"/></figure>


## 3. Repeat (and reflect)
Repeat the steps above for your next two partners' repos. On subsequent loops, note that **after** viewing the project first, you may also want to read and/or refer to the previous comments.

<div class="alert alert-warning">
<strong>Peer reviews are due no later than Thursday at 2:30pm</strong>, so your partners have them for in-class studio.
</div>

But this is not just a way of ensuring that you get feedback from three partners; it's also a way of training your eyes, and of realizing new possibilities. As we head into Thursday's studio class, think about what you've seen that *you'd* like to try. What suggestions would you give yourself?

## EXT: for next time
* As I did at the same point in the visual unit, I'm inviting you to think forward into the final unit, when you'll work to consolidate or build on what you've learned – possibly in partnership with your peers. See <a href="{{site.github.issues_url}}">the issue queue</a> for more details.
* There is no minimum length for this post, but I am interested to see if you're still thinking about logo design and social media campaigns, or if you have something else you'd like to try.
