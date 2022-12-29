# Web unit virtual studio

**Work to have done**:

* Completed the asynchronous workshop in [lesson 20](lesson-20)
* Work in pursuit of a full-draft website that meets [baseline criteria](http://bit.ly/cdm2020spring-criteria#heading=h.z8d1igk08a86)


**Plan for the day**:

1. Welcome back / reminders
2. Screencasts and suchlike resources
3. Set an intention
4. Studio time!
5. Exit note


## 1. Welcome back / reminders
Hello again, everyone! I miss seeing you, but I was very happy to read through your notes to each other on the drafts for Thursday's workshop. If you haven't yet seen or given comments, please try to do so during today's class hours! Instructions are in the [last lesson plan](lesson-20).

<div class="alert alert-success">
Today's studio will work just like last week's. As a reminder, <strong>you are <em>not</em> required to join a Zoom meeting for today's class, but you <em>are</em> expected to post notes on your intention at the beginning and progress by the end of whatever time you spend</strong>; I'll be using those notes as a way of taking today's attendance. Because this is asynchronous, though, you have all of Tuesday to check in. (And if it's there by Wednesday morning, I'll consider it as having been done on Tuesday. :)
</div>

Working on our own times, though, there are still ways to reach out to each other:

* _My online office_, for the duration of the semester, will be at [https://pitt.zoom.us/j/4969331343](https://pitt.zoom.us/j/4969331343). Barring homelife interruptions, I'm going to try to have that room open whenever class would be in session, plus my office hours on Wed/Thurs from 12-1. **I'll be there during today's studio hours, if you want to drop in!** I'm happy to help where I can, and screensharing is often really useful.

* _The google doc_ that we've been using for shared notes, at [http://bit.ly/cdm2020spring-criteria](http://bit.ly/cdm2020spring-criteria), will have new spaces where I'll ask you to check in briefly at the start and end of your own personal class time, mainly during studio days. (See below for some prompts.)

* And of course you can also find each other on GitHub, including on the [Issue Queue]({{site.github.issues_url}}) and the links from there to your various repositories. Filing a help request on the issue queue will be one of the best ways to make sure I help answer your questions: it'll help me keep track of what I've responded to (and what I haven't), and it'll prompt you to give me the info I need to respond more swiftly (like screenshots and links).

## 2. Screencasts and suchlike resources

In the course of responding to questions, I've created a few screencasts, and I'm happy to make more. (I've discovered that Panopto saves straight to Pitt's servers: soo helpful for those of us without room on our harddrives for large video files.)

I'm sharing these here, in case they're helpful to more of you:

* [Putting items in a row with flexbox](https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=bd2f6e85-ddbc-486d-8f92-ab8900188039)
    - Using Flexbox to put images in a horizontal row, rather than displaying as default vertical blocks, takes just one or two lines of CSS and at most two new lines of HTML (<code>&lt;div&gt;</code> and <code>&lt;/div&gt;</code>).
* [Grouping images and captions in rows (HTML/CSS)](https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=ca1c79ce-b1e0-4620-b296-ab8f001a9aef)
    - A block element with `display:flex;` will assign positions to all of its child elements, giving them space based on the *number* of child elements. Therefore, you'll often need to group smaller items into &lt;div&gt;s in order to create the correct number of objects for the flexbox to distribute.
* [Centering a nav-bar with `margin: 0 auto;`](https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=33c892fd-388f-498b-9955-ab8f0015722a)
    - When `margin` (or `padding`) has two values, the first value controls the top-bottom margin (or padding), and the second controls the left-right. `Auto` left-right margins will provide equal spacing (i.e. horizontal centering), but – and here's the kicker – only if the object has a defined width. (Otherwise, your browser won't know how much to subtract from the containing element before splitting that remaining space in half.)

I also highly recommend that you look back over [my expandable notes on the website previews](lesson-19#2-website-construction-seeds-of-revision), from last week's studio, if you haven't yet integrated that cross-project advice:
 * You should have an index.html (or index.md)
 * Don't forget to have alt text for your images
 * Don't forget to update your README.
 * Aim for semanticity: structure in the HTML, display in the CSS.
 * Stuck on layout? Try CSS grid.
 * Take the lowest line-count challenge.

Here's some new advice:
<details>
<summary>If you want to publish your website, use the docs folder</summary>

<p>It's one of the standard places where GitHub pages will look for the files from which to build your site. Inside that folder, you should find a second README that I made with further instructions. (And if you've deleted it, you can look back at <a href="https://github.com/benmiller314/website-portfolio-2020spring/tree/master/docs">the assignment repo</a>.)</p>
</details>

<details>
<summary>Consider leveling up on semantic HTML.</summary>

<p>If you're drowning in "div soup," it may help you to know that HTML5 includes a number of elements that function in basically the same way, but are a lot easier to read: things like <code>&lt;header&gt;</code>, <code>&lt;section&gt;</code>, and <code>&lt;nav&gt;</code>.</p>

<p>Read all about <a href="https://internetingishard.com/html-and-css/semantic-html/">semantic html in the Interneting is Hard tutorial</a>!</p>
</details>

<details>
<summary>Consider titles.</summary>

A title can provide a context, a clue, a genre, a commentary; it can add an extra layer to viewer expectations. In previous units, you were titling your entire project; for a website, every page has its own <code>&lt;title&gt;</code> element in the <code>&lt;head&gt;</code>, which will show up in the browser's tab. These titles <em>could</em> be the same for all your pages, but they could also vary. What text do you want on top of the window, to show users where they are?
</details>

<details>
<summary>Articulate permissions.</summary>

<p>If you're using resources you didn't make yourself, be sure to include enough information to recover where it came from: a direct link to the image and to the specific license (if there is one) is ideal. Where to do this? Ideally, somewhere small under the image itself. (There's a semantic html way of doing this with <code>&lt;figure&gt;</code> and <code>&lt;figcaption&gt;</code>.) Alternately, you can have a rights page somewhere, or use the site footer – or link to an external CREDITS file in your repo.</p>

<p><em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See <em>Writer/Designer</em> page 156 to review the Four Factors you need to consider.</p>
</details>




## 3. Set an intention
<div class="alert alert-success">
Before you start, <a href="http://bit.ly/cdm2020spring-criteria#heading=h.n9upwgwwa42f">head over to the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
  <ul>
    <li>Work on responsive layout?</li>
    <li>Work on making your html match the intended structure?</li>
    <li>Work on replacing placeholder content with real content?</li>
    <li>Work on one of your stretch goals?</li>
    <li>etc etc</li>
  </ul>
Just a sentence or two as a guidepost will give you something to come back to, to reorient, if you find yourself walking in circles or caught in a thicket.
</div>

We're doing this asynchronously now, so I can't keep track of your time... but I can recommend <a href="https://chrome.google.com/webstore/detail/talking-timer-custom-spea/cbbmoeglgokhkbnnfpoeciheapicdphm?hl=en">a Chrome app that will simulate the effect</a>:

<figure>
<img src="../assets/img/custom-talking-timer.png" alt="Talking Timer settings with custom text such as 'it\'s been 25 minutes. Stretch break!' and '15 minutes left. Are you saving and committing?'" />
<figcaption>Custom Speaking Timer. After installing this in Chrome, you can run it standalone from the desktop.</figcaption>
</figure>

I'm sure something similar exists if you're not a Chrome user; I found this one pretty quickly on Google.

## 4. Studio
<div class="alert alert-success">
Take 70 minutes, and subtract however long you just spent reading the advice section above. Then give yourself reminders to stretch, save, and write commit messages as you go!
</div>

I'll be online [in Zoom](https://pitt.zoom.us/j/4969331343) from 2:30-3:45pm.

<div class="alert alert-warning">
Don't forget to save periodically as you go:
 <ul>
   <li>as a project file</li>
   <li>as a git commit, saying what you've just achieved</li>
   <li>as a screenshot</li>
 </ul>
</div>

## 5. Quick report back

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular CSS skill? Decide something about your project? Raise a question in a new way that you'd like some help with?

**Head back into the [google doc](http://bit.ly/cdm2020spring-criteria#heading=h.n9upwgwwa42f) and reply to your intention-post.** You could email me directly if you prefer, but I'm hoping some of your insights or achievements will help inspire others.


# Homework for next time

* Before _Wednesday at 11:59pm_ (a 24-hour blanket extension to allow for wonky work schedules), **push a final-for-now draft of your website to GitHub.** Your repository should include:
   - A multifile **project folder** (probably called "docs"), containing a combination of html, css, and image files
   - At least one more static **<a href="https://www.take-a-screenshot.org/">screenshot</a> (.png or .jpg)** of your web pages in progress.
     * Think about what moments are worth remembering as you go: where did you level up, or realize something, or get stuck?
   - An updated assets or **credits** file reflecting what you actually used, including attribution of any outside sources and your permission to use them (e.g. explicit licenses like CC, or rationales for claiming fair use)
      * If you want, this can be a live page (or a footer) on your website.
   - An updated **README.md** file introducing your website to a new audience. Make it something to live beyond this assignment, if you can. :¬)
* If you're unable to use GitHub right now (because of tech access or other challenges of our new world order), please email me as soon as you can, so we can work something else out.
* Before you start Thursday's class, also **post a prose reflection to the [Issue Queue]({{site.github.issues_url}})** that incorporates images from your feedback and screenshots of your work in progress.
    - Note that "images from your feedback" may now include screenshots of comments from peers – or of messages from me, by email or in lesson plans, if they were helpful!


<div class="alert alert-warning">
Thanks for bearing with me through these weird working conditions, everyone!
</div>
