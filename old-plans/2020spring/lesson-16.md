
# Intro to Web Design and Generative Studio

**Work to have done**:
* As much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-4 (from "Introduction" through "Hello, CSS")

**Plan for the day**:

1. Key Concepts and Practical Takeaways (10-15 min)
2. Web Design in 4 Minutes (10 min)
3. Loop writing (10 min)
4. Offline sketching (10 min)
5. Studio (30 min)

## 1. Key Concepts and Practical Takeaways (10-15 min) <!-- so aim to be done by 2:45 UPDATE actually took until 3:00 -->

At your tables, work through the following questions, and be ready to discuss with the whole class if time allows. Some you should be able to go through rather quickly, while others may require more discussion.

Ask if you can't come to a resolution! I'll share my answer key at the end, so maybe write down your answers for a quick comparison.

Speedy teams, note the EXTs at the end. <!-- and please do skip the EXTs in the middle until you've gone through all the non-EXT questions, just to save time for studio at the end. -->


### Organizing files

1. True or False: filenames are not case sensitive, so it doesn't matter if something is uppercase or lowercase.
2. T / F: web browsers know how to handle spaces in filenames, so it doesn't matter if you have spaces in a filename or not.
3. T / F: all files referred to in an html document have to be in the same folder as that html document.
4. What's one advantage of using a relative link? <!-- easier to change folder names / servers --> What's one risk? <!-- link could break -->
5. EXT: What are some html elements can you use to refer to an external file? (Hint: you should know at least three already.) Where would you put the filename within each of those elements? <!-- <a href="">, <img src="">, <link href=""> -->


### HTML basics
1. What kind of information goes in the `<head>`?
2. How do you mark up comments in HTML?
3. T / F: every HTML element has an opening tag, some element content, and a closing tag.
4. T / F: in rendering an HTML file, there's no difference between a space, a blank line, or five blank lines.
5. EXT: What information should pretty much every page's `<head>` include? <!-- <title>, <meta charset='UTF-8'/> (or whatever actual charset makes sense), <link rel="stylesheet"> -->

### Image basics
1. T / F: every `<img>` tag should specify a source file.
2. T / F: every `<img>` tag should specify a width and a height.
 - EXT: what happens if you only set one?
3. T / F: every `<img>` tag should specify alternative text with `alt`.
4. What makes .jpg files better for photographs than .png files? What makes .png files better for simple diagrams?

### CSS basics
1. Name three different places you could store CSS rules. <!-- external stylesheet, page-specific <style> in the <head>, inline style in the attributes of an html element -->
2. What do the curly brackets in CSS rules do?
3. What do the semicolons in CSS rules do?
4. How do you mark up comments in CSS?
5. How can you apply a single CSS rule to multiple HTML elements?  
6. What happens if you have apply two CSS rules to the same HTML selector, but with different values? <!-- FOR NEXT TIME: cut this question! Or at least save it until after they've read the CSS selectors tutorial. Why is this even here? -->
7. Why is using inline styles generally a bad idea?
8. EXT: What's one advantage of using `em` as a unit rather than `px`? <!-- FOR NEXT TIME: Make this a non-EXT, and add an EXT that follows up on question 1 (i.e. parallel to the EXT for HTML basics), e.g. when would you want to use each of those locations? -->

EXT: If your group finishes early, (a) let me know you're done, and (b) check out these [example web-design sketches](http://designbeep.com/2012/05/17/33-great-examples-of-web-design-sketches/). What design patterns do you notice? What drawing conventions?

EXT: Want to see some sites from past years? Here are a few (more to follow):
* [https://fatemaquaid987.github.io/website/](https://fatemaquaid987.github.io/website/)
* [https://fathimashabnam.github.io/website-portfolio-2019fall/](https://fathimashabnam.github.io/website-portfolio-2019fall/)
* [https://jlatiniii.github.io/website-portfolio-2019fall](https://jlatiniii.github.io/website-portfolio-2019fall)
* [https://pitt-cdm.github.io/website--eaj34/index.html](https://pitt-cdm.github.io/website--eaj34/index.html)
* [https://pitt-cdm.github.io/website--jfrank1120/index.html](https://pitt-cdm.github.io/website--jfrank1120/index.html)

## 1b. If time allows, we can discuss! (5-8 min) <!-- Aim to be done by 2:50... or 3:00 latest! -->
<!-- Answer key below, but also in print-friendly ../uploads/web-tutorial--1-3--answer-key.docx

Organizing files:
1. F: filenames *are* case-sensitive
2. F: it looks ugly with %20
3. F: you can refer to other folders within the root
4. advantage: easier to move the project. risk: link could break silently
5. (EXT) <a href="">, <img src="">, <link href="">

HTML basics
1. metadata!
2. <!-- comments -->
<!-- (oops, gotta restart this comment now)
3. F: trick question. <img />, <br />, and <hr /> are self-closers.
4. True!
5. (EXT) every <head> should include <meta charset='UTF-8'/> and a <title>... and probably a <link rel="stylesheet">

Image basics
1. T: img doesn't function without a src
2. F: width and height are often better set in css
3. T: alt is required.
4. jpgs are lossy, but with photos it's hard to tell. with line diagrams, jpg leads to compression artifacts, and png offers transparency.

CSS basics
1. external stylesheet, page-specific <style> in the <head>, inline style in the attributes of an html element
2. assign rules to selectors / define a ruleset
3. distinguish rules within a ruleset
4. /*  */
5. connect selectors with a comma before a shared set of {}
6. specificity wins; last rule wins.
7. inline styles override the stylesheet, can't make changes in one fell swoop
8. (EXT) em's are way more responsive!
-->

Any tricky ones?
<!-- Ones I think are tricky: Images 2 and 3; CSS 6; -->

## 2. Web Design in 4 Minutes (in 10 minutes) <!-- aiming for 2:50-3:00, END NO LATER THAN no later than 3:05. Move, move, move through the first parts! If you can't start until after 3:00, assign it for homework instead. OOPS, went until 3:20... time to beef up this note...

Better yet, FOR NEXT TIME, just skip this until after they've done the Box Model tutorial, so they know what the heck margin and padding are. Or assign it for homework at that point? As the first part of studio, so people can call you over with questions? This is perhaps better self-paced, because it's obvious to some and opaque to others.
-->

This is what we didn't get to last time. I'm going to try to be brief, but I want to make sure you see this, because many of the suggested design elements / CSS rules make good defaults so your site doesn't look "unstyled."

And now you're in better position to understand the rules as they come up!

[http://jgthms.com/web-design-in-4-minutes](http://jgthms.com/web-design-in-4-minutes/)


## 3. Loop writing (10 min) <!-- aiming for 3:05-3:20 -->
The assignment for Tuesday includes another two chapters in the tutorial, one blog post about advanced CSS selectors, and a proposal for your website project. In a moment, I'll lead you through a generative writing exercise designed to help you come up with an idea to propose.

<div class="alert alert-info">
If you're feeling stuck during the loop writing, you can turn to one of the <a href="https://github.com/benmiller314/website-portfolio-2020spring#parachute-prompts">parachute prompts</a>.
</div>

Take a few minutes to think in writing about the websites you might want to make. I'll read a series of questions aloud. Repeat them silently to yourself, and when you feel yourself answering, make a list.

These lists will remain private, unless you choose to share. I won't ask for them.

1. What have you been working on, in or out of this class, that you'd like to show the world? What have you made, or done, or pursued?
    - Or: if you'd rather the site not focus on _you_, what groups, things, or events might you represent?
2. Is there anything else you might add to the list? A wider context for one of the projects already there, or a related next step?
3. Is there anything you're forgetting? Something you were recently talking about, or planning for? Add it to the list.
    - If you haven't yet included your work for this class, be sure to add it now.

Take a moment now to read back over your lists. **How might you _group_ or _divide_ these items? What clusters do they form?** Mark these in some way.

Is there one cluster that stands out, that says, _me, pick me_? Choose one group to work with, at least for today, and name it in some way. Then copy the name into a clean page.

With that chosen subject, write again:

4. What terms or images come to mind when you think of this subject? ... Think about actions... things... descriptors.
5. I'm going to interrupt you now and ask you to set aside the list, just for now, and ask: **What's the heart of this?** What's the essential component for this cluster of things? What ties them together? <br/><br/>See if you can summon up the whole of this idea, like it's right here in the room with you. Where does it live? Is it above you? Inside you? In the palm of your hand? Just sit with your idea for a moment, feeling where you connect to it.

## 4. Offline sketching (10 min)
And now, draw. Given what's essential, given your knowledge of how websites work, and given the principles of designing for attention we learned last unit, **make a few quick sketches of your possible website's landing page.**

Consider: How will it look on a phone? On a laptop? What might you add to the layout for a full-sized desktop monitor?

Not sure what that should look like? Here are [33 examples](http://designbeep.com/2012/05/17/33-great-examples-of-web-design-sketches/) (but no one is asking you to be as elaborate as the most elaborate of these)

* EXT: Will "inner" pages look the same as the landing page? Sketch out the possible differences. Consider the possibility that someone jumps directly to an inner page (e.g. from Google). What would they need to feel oriented? To get to other pages on the site? (What would you suggest they view next?)
* EXT: Finished one drawing? Make another, using a different system of visually organizing your information.


## 5. Studio / Practice (30 min)

Options!

* Start gathering materials toward your website, to check feasibility.
* If you haven't yet done so, why not start the tutorial sections from the homework?
  - I won't assign *all* the sections of the tutorial; you can look ahead in the [schedule]({{site.github_url}}/schedule) to see which parts I expect you to read and do, and what's beyond baseline.
* Above all, **call me over for help as needed**.

EXT: If you're good on what a CSS class is, and how to add it to an HTML element, read up on [Bootstrap](https://getbootstrap.com/), a very widely used CSS framework. (I use it on this site, for example.) What "framework" essentially means is that they've pre-created a bunch of CSS classes for you, so you can start using them to design your own layout from scratch. It's a little like Lego for web design, only free.


## Homework for Next Time

* **Do** more of the [tutorial](https://internetingishard.com/html-and-css/), getting through at least The Box Model (5) and CSS Selectors (6), if you haven't yet.
* Also **read more** about [how CSS selectors work](https://css-tricks.com/how-css-selectors-work/)
* **Write** a website proposal, posted to the [Issue Queue]({{site.github.issues_url}}/), including:
    - some text about the idea or appeal you're hoping to make;
    - some sense of what pages and page sections you expect to include;
    - a prospective assets chart (what you'll need, where you might get it);
    - at least one design sketch, showing possible layouts; and
    - a link to your repository.
<!-- * When you've finished that, if you haven't yet done so, open the `docs` folder in your forked assignment repo, and read there about how you can take your site public (when you're ready). -->
