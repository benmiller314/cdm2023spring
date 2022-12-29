## How Lo(fi) Should We Go?
**Texts to have read**:

* Stolley, [“The Lo-Fi Manifesto, v. 2.0”](http://kairos.technorhetoric.net/20.2/inventio/stolley/)
* Git Basics videos ["#1 What is VCS?"](https://youtu.be/8oRjP8yj2Wo), ["#4 Quick Wins with Git"](https://youtu.be/7w5Z7LmyLgI), and ["#2 What is Git?"](https://youtu.be/uhtzxPU7Bz0)

**Work to have done**:

* A registered **GitHub** account, with a completed "Hello World" tutorial
* A brief **reflection** posted to the blog under the "reflections" category
* Post three **images** that we can start remixing


## Plan for the Day

### Believing and Doubting Stolley (10-15 min)
Thanks for your reflections! I've seen those that came in by midnight or so. 
Quick favor to me: if you haven't yet done so, please add a category to your post; it helps me justify using WordPress in light of the Voice of Karl Stolley in my head that tells me it's massive overkill for what I need and will trap me in software updates forever.

> Ask someone why they chose a particular technology for a project, and you will often find one little feature driving the decision. It’s astounding, for example, to discover that people choose to set up WordPress to run a small website simply because they wanted a way to repeat the navigation across the four or five pages that made up the site. For that one feature, they pay the tax of securing a database connection and applying software updates for the life of the project, lest the infamous pharma hack or one of its many variants compromise the site. Had such a small site been built with basic HTML, or a static site generator like Jekyll or Wintersmith, no updates beyond those routine to the web server itself would likely be needed.

Ugh, it's like a dagger to the heart!

* Brief spiel on believing and doubting (Elbow)
* If we play the believing game with Stolley, what's the takeaway?
* If we play the doubting game with Stolley, what's the takeaway?
* What questions do you have?
 
EXT: Did anyone notice the little link at the top to the [Readme](http://kairos.technorhetoric.net/20.2/inventio/stolley/readme/) page? How, if at all, does that page change your sense of the article?

EXT: Let's think about genre and audience for a moment. This was published in the same venue as Sorapure's Flash-or-PDF piece about the Five Principles of New Media: the online-only academic journal <em>Kairos: A Journal of Rhetoric, Technology, and Pedagogy</em>. 


#### Is version-control just for code?

* Let's have a look at [Stolley's revision history](https://github.com/karlstolley/lo-fi/commits/master/stolley/index.html).
* Despite what you may read in some old websites (a reminder that Google is not always an infallible source of up-to-date information), GitHub can handle images – and even show [differences between versions](https://github.com/blog/817-behold-image-view-modes). However, this is only true of "lo-fi" *individual image files* – not "hi-fi" project files that contain multitudes of images within them.
* Side note: some of you may be interested in [draftin.com](https://draftin.com)


### Studio time: Practice with GIMP / Photoshop (30 min)

As you might imagine, this is one of those hi-fi tools that Stolley was talking about: the GUI interface that "hides" what's going on behind the curtain, the complicated array of buttons that will probably change every time there's a new version.

I'm not interested in your mastering this particular piece of software. What I'm after, instead, is the *kind* of things it can do, wants to do, makes easy to do – that is, what actions the tool *affords*.

<!-- NOTE for next time: instead of dumping them into GIMP, 
1. do an offline activity that clarifies the concept of *layers*
2. demo and have them imitate one common image editing task: removing / changing the background -->

<div class="alert alert-info">
<ol>
<li>Pick a few images to work with from the galleries below, and download them to a scratch space.</li>
<li>Open GIMP (or Photoshop, if GIMP isn't here yet) and File > Import as Layers</li>
<li>Play around with layers and selections to get a sense of what it can do<ul><li>ALT:if you're already familiar with image editing tools, have some fun with your files! Show off to or give guidance to your classmates!</li></ul></li>
<li>Have a look at your revision history. In what ways is this like what Git lets you do? In what ways is it different? Can you think of any ways to combine the two?</li>
<li>When you've had a chance to play around for a while, <em>save the project</em> to your Box/Dropbox/Drive, <strong>and</strong> <em>export the image</em> as a .png file.</li>
</ol>
</div>

For more on image file formats, try a search for the options you're curious about – there's lots on wikipedia, e.g. – or start with the top two results on this Stack Overflow thread: ["What is the difference between “JPG” / “JPEG” / “PNG” / “BMP” / “GIF” / “TIFF” Image?"](https://stackoverflow.com/questions/419584/what-is-the-difference-between-jpg-jpeg-png-bmp-gif-tiff-i) 


#### Galleries!

I'm further taking advantage of the affordances of WordPress and dynamically querying the database to pull out every image within the three Asset categories we've assigned so far. When you add a new image, the galleries will update. (And, because this gallery type likes to make one image more prominent than the others, I've told it to randomize: every time you refresh or revisit the page, it'll have a different image in the featured slot.)

##### Actions

[gallery orderby="rand" type="rectangular" media_category="12"]

##### Emotions

[gallery orderby="rand" type="rectangular" type="square" media_category="13"]

##### Settings

[gallery orderby="rand" type="rectangular" media_category="14"]


### Studio Time: Working with Git / GitHub
I want to suggest that you commit your changes to the image files you're working on, both to get comfortable working with the system, and to get you into the habit of saving a commit message every so often. (So much better than just hitting save and overwriting your previous iteration, and having no idea when you come back to it, two days or two weeks or even two months later, what you were actually working on.)

BUT I'm not sure if these lab computers have Git installed, or if they'll let you install it if they don't. SO if you have your own computer, by all means proceed!

Here's a super-quick [installation overview](https://gist.github.com/derhuerst/1b15ff4652a867391f03) (posted using GitHub's "gist" system for publishing quick one-page snippets).

Alternately, you can download the [GitHub desktop application](https://desktop.github.com/), which, despite Gabi's legitimate concern that we [get over any fears of the command line](https://cdm2017.majoringinmeta.net/an-argument-for-lo-fi-github-use-and-learning-more-about-your-computer-generally/), is actually quite handy for partial-file commits and intuitive diff views. Yeah, it can't do everything; it can get you more comfortable with the flow, so you know what commands to *want* to give in the command line.


If all else fails, you can use the GUI on [the GitHub website](https://github.com) to create a new repository ("repo") and upload files to it, with commit messages. This approach has limits: for one, it's a lot harder to wrap several file changes in a single commit.


I'll float around and see where I can be helpful!

EXT: there's always the option, in a studio class, to start on the homework.


## Homework for Next Time

* **Administrative**
 1. If you haven't yet, please **fill out** the [Tech Comfort Survey](https://goo.gl/forms/Y6SZfG9Od2JUw1y42).
 2. If you have filled out the survey, please **[schedule a conference](https://benmiller314.youcanbook.me)** with me at your convenience. 
 3. **Install** GIMP on a machine that you're likely to use at home
* **Inputs**
 1. **Read** pages 63-76 in *Writer/Designer*, which is part of chapter 4. It deals with "Ethics of Collecting Sources and Assets." 
 2. **Read** quickly through the Stanford library's [website on Copyright and Fair Use](http://fairuse.stanford.edu/overview/), paying particular attention to the section on [Measuring Fair Use: the Four Factors](http://fairuse.stanford.edu/overview/fair-use/four-factors/) and anything else that seems especially pertinent to you.
 3. EXT: **Watch** an introductory tutorial on GIMP if you want something extra to help you get oriented. There's a Lynda tutorial called ["GIMP Essential Training"](https://www.lynda.com/GIMP-tutorials/Touring-GIMP-interface/572891/626849-4.html) that covers a *lot* (it's like 5 hours long), but starts with a 5 *minute* intro to the interface.
  * You can access Lynda tutorials through [my.pitt.edu](https://my.pitt.edu); look for the link in the sidebar. ![lynda link, screenshot from my.pitt sidebar](assets/img/lynda-link.png)
* **Outputs**
 1. **Consider**: where did you find the images you posted for lesson 3? Are you able to get back to them easily? Did you embed any citation information when you posted them to our website? Do you have permission to reuse or modify these images? 
 2. **Update or change** the info in our media library, as necessary. (Go to the dashboard, then Media, then Library, and use the filters to navigate.)
 3. **Write** any questions you have so far – about any of our readings, but perhaps especially about ethical sourcing – and post them to our blog under the Reflections category.
