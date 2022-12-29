
# Core Concepts of HTML & CSS + Studio

**Work to have done**:
* As much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-4 (from "Introduction" through "Hello, CSS"); _push your tutorial code to GH_

**Plan for the day**:

1. Key Concepts and Practical Takeaways (20-30 min)
2. Intro to studio
3. Studio (25 min)

## 1. Key Concepts and Practical Takeaways (20-30 min) <!-- so for a 1:00 start, aim to be done by 3:25 -->

In groups at your tables, work through the following questions, and be ready to discuss with the whole class if time allows. Some you should be able to go through rather quickly, while others may require more discussion. (For example, some of the True/False questions are actually a little subtler than that framing suggests: e.g. *mostly* true, except when ____.)

<div class="alert alert-success">
<strong>Please take turns within your group</strong> reading questions and proposing answers, so that everyone in the group bears responsibility. <!--Also, to help me keep track of where everyone's up to, <strong>please take notes in the <a href="http://bit.ly/cdm2022spring-notes">shared google doc</a></strong> -->.
</div>

**Speedy teams, note the EXTs** at the end. Conversely, feel free to **skip the EXTs in the middle if you're running behind** – we want to make sure you have enough writing time in the second part of class.

Call me in if you can't come to a resolution! I will share my answer key at the end.

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


<!-- 6. What happens if you have apply two CSS rules to the same HTML selector, but with different values? <!-- FROM LAST TIME: cut this question! Or at least save it until after they've read the CSS selectors tutorial. Why is this even here? -->



<div class="alert alert-info">
<p>If your group finishes early, (a) let me know you're done, (b) <a href="../uploads/lesson-17--web--answer-key.docx">download my answer key</a> and confirm we're on the same page. If not, let me know that, too!</p>

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


## 3. Studio / Practice (45-60 min) <!-- for a 1:00 start, you have to get here by 1:25, ending by 3:35 -->

<div class="alert alert-success">See below for options, then please go to <a href="https://bit.ly/cdm2022spring-notes#heading=h.hiw73w6fl2zt">bit.ly/cdm2022spring-notes</a> and let me know what you're working on; this helps me figure out where I can be most helpful.</div>

1. **If your tutorial pages aren't looking like the examples, tell me now, so I can help you get there!** You'll get a lot more out of the later tutorials if you've got these first ones solidly under your belt.

2. The assignment for Thursday includes another two chapters in the tutorial and a game to play (or a blog post to read) about more advanced CSS selectors. If you haven't yet done so, why not start those homework assignments?

3. If you're feeling good about all that, start translating your website sketches – especially your website *content* – into HTML and then CSS. Begin by adapting the tutorials, once you know you've got them working, to include your own materials.
  - Use the _docs_ folder for files you'll eventually want to publish on the web.
  - Call the file for your landing/home page **index.html**. You can always change the `<title>`.

4. Above all, call me over for help as needed.

EXT: If you've already done the above, and you're good on what a CSS class is, and how to add it to an HTML element, read up on [CSS frameworks]({{site.github_url}}/resources#frameworks) on our course Resources page. They're basically a bunch of pre-created CSS classes you can use to design your own layout from scratch: a little like Lego for web design. (I use the Bootstrap framework on this site.)


## Homework for Next Time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), getting through at least The Box Model (5) and CSS Selectors (6), if you haven't yet.
  - Remember that I won't assign *all* the sections of the tutorial; you can look ahead in the [schedule]({{site.github_url}}/schedule#unit-4) to see which parts I expect you to read and do, and what's beyond baseline. You can probably skip Floats.
* Please do, though **read** more about [how CSS selectors work](https://css-tricks.com/how-css-selectors-work/) *OR* if you prefer game-based learning to straight-up reading, try loading and clearing plates at the [CSS Diner](https://flukeout.github.io/). (There's still reading, in the sidebar, which tells you how to win the round.)
* As you're able to get the tutorials working, you can start adapting the files there to include your own content; save those more personal files in the _docs_ folder.
