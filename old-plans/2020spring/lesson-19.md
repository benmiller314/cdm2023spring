# Web unit virtual studio

**Work to have done**:

* Progress in the [html + css tutorial](https://internetingishard.com/html-and-css/), up to the section on semantic html
* Work in pursuit of a full-draft website that meets [baseline criteria](http://bit.ly/cdm2020spring-criteria#heading=h.z8d1igk08a86)


**Plan for the day**:

1. Welcome back (and important links)
2. Website construction: seeds of revision
3. Set an intention
4. Studio time!
5. Exit note


## 1. Welcome back (and important links)
Welcome back, everyone – if your last two weeks have been anything like mine, they've been full of anxious news-reading, rebuilding in the wake of disrupted plans, and what one professor I used to work with called "Forced Family Fun."

I'm expecting a certain amount of flexible asynchronicity to the lesson plans moving forward, so adjust to the time you have available. That said, I also want to maintain **a few online spaces where we can feel connected to one another:**

* _My online office_, for the duration of the semester, will be at [https://pitt.zoom.us/j/4969331343](https://pitt.zoom.us/j/4969331343). Barring homelife interruptions, I'm going to try to have that room open whenever class would be in session, plus my office hours on Wed/Thurs from 12-1. **Please come find me there during today's studio hours!** I'm happy to help where I can, and screensharing is often really useful.

* _The google doc_ that we've been using for shared notes, at [http://bit.ly/cdm2020spring-criteria](http://bit.ly/cdm2020spring-criteria), will have new spaces where I'll ask you to check in briefly at the start and end of your own personal class time, mainly during studio days. (See below for some prompts.)

* And of course you can also find each other on GitHub, including on the [Issue Queue]({{site.github.issues_url}}) and the links from there to your various repositories. Filing a help request on the issue queue will be one of the best ways to make sure I help answer your questions: it'll help me keep track of what I've responded to (and what I haven't), and it'll prompt you to give me the info I need to respond more swiftly (like screenshots and links).


## 2. Website construction: seeds of revision

Today is all about working on your individual projects! Add and mark up content, adjust layout, watch relevant tutorials. I know your lives are busy, especially now; hopefully you have a space and time when you can get free from other distractions and obligations to move your composition forward.

Here are some cross-project ideas to think about as you engage with the particulars of your own:

<details>
<summary>You should have an index.html (or index.md)</summary>
By default, this is what a web browser will display when you just type in the URL of your website: it is, in other words, the default filename for your home page. If your home page currently has another filename, <a href="https://www.lifewire.com/index-html-page-3466505">you probably want to change it to index.html</a>. You can always keep your more interesting name as the &lt;title&gt;!
</details>

<details>
<summary>Don't forget to have alt text for your images</summary>
Text-alternatives, which you add to images using <code>&lt;img alt="text description here" src="path/to/source.jpg"&gt;</code>, are a required element in validated html. They're also really helpful, and not only to blind users: they make the html file more readable on its own, and thus more semantic, and they help you troubleshoot layout when image paths are broken by showing you where each image is trying to appear. For more guidance on how to write useful alt text, see <a href="https://webaim.org/techniques/alttext/">https://webaim.org/techniques/alttext/</a>.
</details>

<details>
<summary>Don't forget to update your README.</summary>
This is what GitHub Pages will display if you don't have an index file, but it's also a kind of cover letter for your code. The README should have a brief description of the project, and may I also suggest an active link to your live website, if you have one?
</details>


<details>
<summary>Aim for semanticity: structure in the HTML, display in the CSS.</summary>

<p>If you have hard-coded display using HTML elements like &lt;center&gt;, &lt;font&gt;, or &lt;b&gt;, or if you have inline style set with the "style" attribute on individual elements, I encourage you to look for ways to do this instead with CSS. This is a matter of both flexibility and accessibility, and it makes it a lot easier to revise if you later decide to, say, change your color scheme: you just have to change one line in the CSS, rather than search for every explicit tag.</p>

<p>For some things, this separation even makes it easier to decide what you want: you can play with the CSS rules (and select colors!) directly in the browser's inspector, and then grab what you want. Firefox is especially user-friendly for this. See <a href="lesson-18">last class's lesson plan</a> (wow, that was a long time ago) for a gif of what this might look like.</p>
</details>

<details>
<summary>Stuck on layout? Try CSS grid.</summary>

<p>I assigned <a href="https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725">a great Medium post introducing the reader to CSS Grid</a> as homework after lesson 17, but it's probably worth revisiting now that you've had a little more experience. The latest CSS approach to layout, Grid is new enough that it's not in the "Interneting is Hard" tutorial, but old enough that it's now has almost universal browser support.</p>

<p>What I like about this particular tutorial – just a 7-minute read, the header helpfully informs me – is that it's embedded not only with images, but with short screen-capture GIFs that demonstrate in a very immediate way what happens to the layout when a new CSS rule is added.</p>

<p>Author Rafaela Ferro also does a great job of keeping the tone light by focusing on cute pictures of dogs. I also recommend her follow-up tutorial on <a href="https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f">using CSS Grid to create responsive layout</a> – which is, she argues, even easier to do with Grid than with Flexbox (let alone Float).</p>

</details>


<details>
<summary>Take the lowest line-count challenge.</summary>
<p>In the HTML, consider whether you need all the &lt;div&gt;s you have, or whether you could put the relevant class directly on the element inside it. (You might well need the container for flexbox or grid layout.) The way I think of &lt;div&gt; is that it groups together several items, kind of like the "group" button in PowerPoint or the layer-groups in GIMP: if you only have one thing inside a &lt;div&gt;, you probably don't need it.</p>

<p>In CSS, look for ways to consolidate rules to avoid repeating yourself. For example, any style you need to apply more than once should probably use a <em>class</em> selector that you can re-use several times in your HTML, rather than an <em>id</em> (which you can only use once).</p>

<p>Bear in mind that the <em>cascading</em> aspect of CSS means you can combine rules, so <strong>you can define a general class for (say) images and then add or override just one or two lines for a subclass:</strong></p>

<figure>
<img src="../assets/img/multiclass-css.jpg" alt="example of html element with two css classes." />
<figcaption>Use a space between the several classes.</figcaption>
</figure>

<p>Rules at the same level of specificity will be applied in the order they appear in the CSS, so later rules override over earlier ones.</p>
</details>


<!--
<summary>Consider leveling up on semantic HTML.</summary>

<p>If you're drowning in "div soup," it may help you to know that HTML5 includes a number of elements that function in basically the same way, but are a lot easier to read: things like <code>&lt;header&gt;</code>, <code>&lt;section&gt;</code>, and <code>&lt;nav&gt;</code>.</p>

<p>Read all about <a href="https://internetingishard.com/html-and-css/semantic-html/">semantic html in the Interneting is Hard tutorial</a>!</p>
</details>


<details>
<summary>Articulate permissions.</summary>

<p>If you're using resources you didn't make yourself, be sure to include enough information to recover where it came from: a direct link to the image and to the specific license (if there is one) is ideal. Where to do this? Ideally, somewhere small under the image itself. (There's a semantic html way of doing this with &lt;figure&gt; and &lt;figcaption&gt;.) Alternately, you can have a rights page somewhere, or use the site footer – or link to an external CREDITS file in your repo.</p>

<p><em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See <em>Writer/Designer</em> page 156 to review the Four Factors you need to consider.</p>
</details>

<details>
<summary>Consider titles.</summary>

A title can provide a context, a clue, a genre, a commentary; it can add an extra layer to viewer expectations. In previous units, you were titling your entire project; for a website, every page has its own <code>&lt;title&gt;</code> element in the <code>&lt;head&gt;</code>, which will show up in the browser's tab. These titles <em>could</em> be the same for all your pages, but they could also vary. What text do you want on top of the window, to show users where they are?
</details>

-->


## 3. Set an intention
<div class="alert alert-success">
Before you start, <a href="http://bit.ly/cdm2020spring-criteria#heading=h.qobrtj4szd0b">head over to the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
  <ul>
    <li>Work on responsive layout?</li>
    <li>Work on replacing placeholder content with real content?</li>
    <li>Work on streamlining your code?</li>
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

<div class="alert alert-success">
Take 70 minutes, and subtract however long you just spent reading the advice section above. Then give yourself reminders to stretch, save, and write commit messages as you go!
</div>

<div class="alert alert-warning">
Don't forget to save periodically as you go:
 <ul>
   <li>as files in Atom</li>
   <li>as a git commit, saying what you've just achieved</li>
   <li>as screenshots of either your workspace or your site-in-progress</li>
 </ul>
</div>

## Quick report back

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular CSS skill? Decide something about your project? Raise a question in a new way that you'd like some help with?

**Head back into the [google doc](http://bit.ly/cdm2020spring-criteria#heading=h.qobrtj4szd0b) and reply to your intention-post.** You could email me directly if you prefer, but I'm hoping some of your insights or achievements will help inspire others.


# Homework for next time

* Before Thursday at 10am, **push a full draft of your website to GitHub.** Your repository should include:
   - A multifile **project folder** (probably called "docs"), containing a combination of html, css, and image files
   - At least one more static **<a href="https://www.take-a-screenshot.org/">screenshot</a> (.png or .jpg)** of your web pages in progress.
     * Think about what moments are worth remembering as you go: where did you level up, or realize something, or get stuck?
   - An updated assets or **credits** file reflecting what you actually used, including attribution of any outside sources and your permission to use them (e.g. explicit licenses like CC, or rationales for claiming fair use)
      * If you want, this can be a live page (or a footer) on your website.
   - An updated **README.md** file introducing your website to a new audience. Make it something to live beyond this assignment, if you can. :¬)
* Because we're working remotely, it's essential for Thursday's workshop that your repo be in clonable condition. You can check by cloning it again yourself to a different location on your computer: if you can open the files in that new location without a problem, you're good to go. (And good as well to delete your duplicate copy, before you forget which files you were updating.)
* If you're unable to use GitHub right now (because of tech access or other challenges of our new world order), please email me as soon as you can, so we can work something else out.
* I'll let you know by Thursday morning which repos you'll be responding to, and on Thursday's lesson plan I'll have instructions for how to comment.

_Thanks for bearing with me through these weird working conditions, everyone!_
