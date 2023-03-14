
# Core Concepts of HTML & CSS + Studio

<div class="alert alert-warning">We've had a request to activate the Zoom today. Please remind me if I forget?</div>

**Work to have done**:
* As much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-4 (from "Introduction" through "Hello, CSS"); _push your tutorial code to GH_

**Plan for the day**:

0. Upcoming workshops (5 min)
1. Key Concepts and Practical Takeaways (20-30 min)
2. Intro to studio (5 min)
3. Studio (35-45 min)

## 0. Announcement: Accessible Web Design workshops 

There's a series of workshops this Friday (html) and next (css), right here in this room, from 2:30-3:30, aimed at ways to make the web more navigable by more people. They're hosted by Lynn Priestley – who is, among other things, author of the [Loose Leaf cafe](https://cap-alt-delete.github.io/website-portfolio-2021spring/) website that I gave you as an example. She's also the host of a podcast on this subject, [Welcomed by Design](https://open.spotify.com/show/2fiqvtqdyyZfpGATtPLpgl?si=8582cbb529574d53). 

If you can make the time, I highly encourage you to [register using this link](https://docs.google.com/forms/d/e/1FAIpQLSfPzuLPbCkRQ7k4--R8Ti7zkM1zzLP-jlZ7MwQIShlyeiU6Kw/viewform) to get demo / practice files! Here's a [flyer with more information](../uploads/AccessibleWebWorkshops.pdf). <span class="sr-only">And here's a background image description for the flyer, which should otherwise have embedded text accessible: Abstract, color-block representation of a desktop computer screen, with the introductory text placed on the main web page. The event details are on a coding sidebar, with the who/what/where/preregister headings wrapped to look like HTML tags. End of image description.</span>


There's also a workshop this Friday morning, 11:00-1:00, on _Alt-Text as Poetry_, hosted by the artist, writer, and disability activist Bojana Coklyat. That's across the street in 527 William Pitt Union. This workshop will be capped at 20 and is open to anyone at the university, though priority will be given to graduate and upper-level undergraduate students. You can [register here](https://pitt.co1.qualtrics.com/jfe/form/SV_6znqFaKfKQgazem).



## 1. Key Concepts and Practical Takeaways (20-30 min) <!-- so for a 1:00 start, aim to be done by 3:25 In 2023, we start the solo round at around 1:10. All groups talking by 1:23. -->
<div class="alert alert-success">
Start by answering each of the questions below <strong>on your own</strong> (skipping the EXTs for now). Write down your answers in your own space. <!-- FOR NEXT TIME: Have a downloadable quiz sheet so people don't feel like they have to waste time copying stuff out -->
</div>
<p>(Note that some of the True/False questions are actually a little subtler than that framing suggests: e.g. *mostly* true, except when ____.)</p>


Then **discuss your answers in groups** at your tables, and be ready to discuss tricky ones with the whole class if time allows. Some you should be able to go through rather quickly, while others may require more discussion. 

<div class="alert alert-success">
<strong>Please take turns within your group</strong> reading questions and proposing answers, so that everyone in the group bears responsibility. <!--Also, to help me keep track of where everyone's up to, <strong>please take notes in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">shared google doc</a></strong> -->.
</div>

**Speedy teams, note the EXTs** at the end. Conversely, feel free to **skip the EXTs in the middle if you're running behind** – we want to make sure you have enough working time in the second part of class.

Call me in if you can't come to a resolution! I will share my answer key when your table is ready.

<!-- <div class="alert alert-warning">
To get async credit for this portion of the class, please answer these questions in your own space (i.e. not in the gdoc) and send your answers my way.

You'll also want to do the generative exercise a bit further down!
</div> -->


### Organizing files

1. True or False: filenames are not case sensitive, so it doesn't matter if something is uppercase or lowercase.
2. T / F: web browsers know how to handle spaces in filenames, so it doesn't matter if you have spaces in a filename or not.
3. T / F: all files referred to in an html document have to be in the same folder as that html document.
4. What's one advantage of using a relative link? <!-- easier to change folder names / servers --> What's one risk? <!-- link could break, especially if you shift folder nesting levels -->

EXT: What are some html elements can you use to refer to an external file? (Hint: you should know at least three already.) Where would you put the filename within each of those elements? <!-- <a href="">, <img src="">, <link href=""> -->


### HTML basics
1. What kind of information goes in the `<head>`?
2. How do you mark up comments in HTML?
3. T / F: every HTML element has an opening tag, some element content, and a closing tag.
4. T / F: in rendering an HTML file, there's no difference between a space, a blank line, or five blank lines.

EXT: What three tags should pretty much every published page's `<head>` include? <!-- <title>, <meta charset='UTF-8'/> (or whatever actual charset makes sense), <link rel="stylesheet"> -->

### Image basics
1. T / F: every `<img>` tag should specify a source file.
2. T / F: every `<img>` tag should specify a width and a height.
    - What happens if you only set one?
3. T / F: every `<img>` tag should specify alternative text with `alt`.

EXT: What makes .jpg files better for photographs than .png files? What makes .png files better for simple diagrams?

### CSS basics
1. What do the curly brackets and semicolons in CSS rules do?
2. How can you apply a single CSS rule to multiple selectors?  
3. How do you mark up comments in CSS?
    - EXT: what's the shortcut in your text editor for (un)commenting out the current line?
4. Name three different places you could store CSS rules. <!-- external stylesheet, page-specific <style> in the <head>, inline style in the attributes of an html element -->
5. Why is it generally a bad idea to use inline styles?

EXT: Given the three locations in question 4, when would you want to use each? What are the pros and cons?



<div class="alert alert-info">
<p>If your group finishes early, (a) let me know you're done, (b) <a href="../uploads">download my answer key</a> and confirm we're on the same page. If not, let me know that, too!</p>

<p>Then (c) try the EXT activities below while you wait for the other groups to catch up.</p>
</div>



<!-- EXT 1: Flip through these <a href="http://designbeep.com/2012/05/17/33-great-examples-of-web-design-sketches/">example web-design sketches</a>. What design patterns do you notice? What drawing conventions? -->


EXT: Talk through the example sites from last year (from HW reading before break, and pasted again below for convenience), looking at the HTML with either View Source or your browser's inspector. How are the pages structured? Any surprises? Any changes you'd want to make? Anything you'd want to borrow for your own site?
<details><summary>Convenient links</summary>
<ul><li> <a href="https://fatemaquaid987.github.io/website/index.html">Fatema Quaid</a>, by Fatema Quaid</li>
<li><a href="https://cmgo412.github.io/website-portfolio-2021spring/">Hi, I'm Caela</a>, by Caela Go</li>
<li><a href="https://cap-alt-delete.github.io/website-portfolio-2021spring/">Loose Leaf</a>, by Lynn Priestley</li>
<li><a href="https://shreyababu.github.io/website-portfolio-2020fall">The Rwandan Genocide: 100 Days of Silence</a>, by Shreya Babu</li>
</ul>
</details>

## 2. Anything to discuss further? (5-8 min) <!-- for a 1:00 start, you have to move on no later than 1:35. So aim to start discussion no later than 1:20... 1:15 would be better -->

Let me know if you have any challenges or questions after reading my answer key!


## 3. Studio / Practice (45-60 min) <!-- for a 1:00 start, you have to get here by 1:25, ending by 1:35 -->

<div class="alert alert-success">See below for options, then please go to <a href="https://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.hiw73w6fl2zt#heading=h.jf786cdz1a2q">bit.ly/cdm{{site.course.slugterm}}-notes</a> and let me know what you're working on; this helps me figure out where I can be most helpful.</div>

1. **If your tutorial pages aren't looking like the examples, tell me now, so I can help you get there!** You'll get a lot more out of the later tutorials if you've got these first ones solidly under your belt.

2. The assignment for Thursday includes another two chapters in the tutorial and a game to play (or a blog post to read) about more advanced CSS selectors. If you haven't yet done so, why not start those homework assignments?

3. If you're feeling good about all that, start translating your website sketches – especially your website *content* – into HTML and then CSS. Begin by adapting the tutorials, once you know you've got them working, to include your own materials.
    - Use the _docs_ folder for files you'll eventually want to publish on the web.
    - Call the file for your landing/home page **index.html**. You can always change the `<title>`.

4. Above all, call me over for help as needed.

EXT: If you've already done the above, and you're good on what a CSS class is, and how to add it to an HTML element, read up on [CSS frameworks]({{site.github_url}}/resources#frameworks) on our course Resources page. They're basically a bunch of pre-created CSS classes you can use to design your own layout from scratch: a little like Lego for web design. (I use the Bootstrap framework on this site.)


## Homework for Next Time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), getting through at least The Box Model (5) and CSS Selectors (6), if you haven't yet.
  - Remember that I won't assign *all* the sections of the tutorial; you can look ahead in the [schedule]({{site.github_url}}/schedule#current) to see which parts I expect you to read and do, and what's beyond baseline. You can probably skip Floats, for example... and I'll ask you to look at some Grid tutorials that aren't part of the main series.
* Please do, though **read** more about [how CSS selectors work](https://css-tricks.com/how-css-selectors-work/) *OR* if you prefer game-based learning to straight-up reading, try loading and clearing plates at the delightful [CSS Diner](https://flukeout.github.io/). (There's still reading, in the sidebar, which tells you how to win the round.)
* As you're able to get the tutorials working, you can start adapting the files there to include your own content; save those more personalized files in the _docs_ folder.
  - Save and commit as you go!

<!-- * **View** screencast on using <nav><ul><li></a> and CSS to remove bullets ... and to resize the <a> directly using padding. Point out that this is a direct application of the Box Model. -->

Pi Day bonus! [https://www.youtube.com/watch?v=NmxPeBeX_38](LullaPi: A Piano Piece Inspired by the digits of Pi)