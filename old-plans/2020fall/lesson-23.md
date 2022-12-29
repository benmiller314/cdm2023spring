
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

As a reminder, here's my [general advice already given](lesson-19):
* When revising, take the lowest line-count challenge
* Let appearances (CSS) reflect the structure (HTML), not vice-versa
* Consider leveling up on semantic HTML elements like `<nav>` and `<section>` (especially if you're drowning in div soup)
* Stuck for what to do, CSS-wise? Start with some basic spacing

In addition, I hope you can...
<details>
<summary>Articulate permissions.</summary>

<p>If you're using resources you didn't make yourself, be sure to include enough information to recover where it came from: a direct link to the image and to the specific license (if there is one) is ideal. Where to do this? Ideally, somewhere small under the image itself. (There's a semantic html way of doing this with &lt;figure&gt; and &lt;figcaption&gt;.) Alternately, you can have a rights page somewhere, or use the site footer – or link to an external CREDITS file in your repo.</p>

<p><em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See <em>Writer/Designer</em> page 156 to review the Four Factors you need to consider.</p>
</details>

<details>
<summary>Call your homepage index.html (or index.md)</summary>
By default, this is what a web browser will display when you just type in the URL of your website: it is, in other words, the default filename for your home page. If your home page currently has another filename, <a href="https://www.lifewire.com/index-html-page-3466505">you probably want to change it to index.html</a>. You can always keep your more interesting name as the &lt;title&gt;!
</details>

<details>
<summary>Have alt text for all your images</summary>
<p>Text-alternatives, which you add to images using <code>&lt;img alt="text description here" src="path/to/source.jpg"&gt;</code>, are a required element in validated html. They're also really helpful, and not only to blind users: they make the html file more readable on its own, and thus more semantic, and they help you troubleshoot layout when image paths are broken by showing you where each image is trying to appear.</p>

<p>For more guidance on how to write useful alt text, see <a href="https://webaim.org/techniques/alttext/">https://webaim.org/techniques/alttext/</a>.</p>
</details>

<details>
<summary>Remember to update your README.</summary>
It should have a brief description of the project, and may I also suggest an active link to your live website, if you have one?
</details>

<details>
<summary>Consider titles.</summary>

A title can provide a context, a clue, a genre, a commentary; it can add an extra layer to viewer expectations. In previous units, you were titling your entire project; for a website, every page has its own <code>&lt;title&gt;</code> element in the <code>&lt;head&gt;</code>, which will show up in the browser's tab. These titles <em>could</em> be the same for all your pages, but they could also vary. What text do you want on top of the window, to show users where they are?
</details>



## Gathering questions

As you finish taking in the advice of your peers (and going over my suggestions above), I'd like to know **what questions you have that I might be able to help with** – especially if it's about something you've seen in assigned readings or revision suggestions, but you're not sure how to implement.

Head into [the google doc](http://bit.ly/cdm2020fall-notes) and write down what you're thinking about. It can be anonymous!

If clusters start to form, I can create breakout groups where we can work on those things together.

Otherwise, I might just create a room for everyone to hang out in – as if it were pre-COVID times! sigh – and we can all hear questions as they come up; if the answers are involved, or need screensharing, those of us who are interested can come back to the main room to work through it. (This will allow people to still call me back into a breakout room for a different question, something the old system of coming into the main room to look for me couldn't do.)


## Studio Time!

### Set an intention
As usual, before you start, <a href="http://bit.ly/cdm2020fall-notes">go to the next section of the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
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
* By Tuesday's class, **write a prose reflection** that incorporates images from your feedback and screenshots of your Atom project and the website itself. As explained in the [prompt for the assignment](https://github.com/benmiller314/website-portfolio-2020fall#project-3-website-portfolio), this should include:
   - At least 500 words
   - Your own assessment of how you met the baseline criteria and goals for the unit, as well as any aspirational criteria as appropriate
   - At least one photograph of a notecard with feedback you used (and please say how)
   - At least one or two screenshots of your work in progress (ideally, related to the discussion in the previous two bullets)
* **Post your reflection** to the course site's [Issue queue]({{site.github.issues_url}}/14), to make it easier to embed images.
   - If you want to then copy the source code into a file in your repo called reflections.md, I won't stop you!
   - If you feel strongly that you'd rather keep your reflection private, you can email it to me instead. But my default assumption is that we learn from each other as much as from ourselves, so I hope you can find a way to write publicly about your experience with this project.
   
