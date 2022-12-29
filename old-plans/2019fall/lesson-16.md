---
layout: bottomnav
---


# Midterm Reflections and Intro to Markup

**Work to have done**:

* Your final-for-now Visual Rhetorical Collage and Reflection
* Download and install the [Atom text editor](http://atom.io)

**Plan for the day**:

1. Midterm reflection (5-10 min)
2. Web-design unit overview and assignment (10 min)
3. Markup: separating content from display (10-15 min)
5. Homework preview

<!-- NOTE FOR NEXT TIME: don't cut CSS in 4 minutes, and maybe even start with it? I ended up with 30 minutes left!!

Okay, here's my current proposal for next time:
1. midterm reflection (10 min)
2. share / discuss reflections (10 min)
3. CSS Zen Garden. (5 min) different ways visual representations can highlight / draw attention.
4. Reveal: every one of these sites uses the exact same underlying text. How? By telling the computer what _parts_ a thing has, you can separate out how to _display_ those parts.
Consider making a PowerPoint for the next bit:
5. Separate, but cross-related, languages have developed to handle the part-marking and the display: html and css. (other web languages, like php, javascript, ruby, and python, can dynamically generate or change the html and css; but html and css are the core of what gets shown on the screen.)
6. pre-fab (not inspector-based) examples (maybe in a codepen?) of html + css + output. structure of an html tag (maybe start with <a>, because it has attributes? use atom to show syntax highlighting, which makes it easier to see the parts. also note the open-tag close-tag structure is essentially like parentheses, and show https://xkcd.com/859/.)
7. div as a kind of layer-group: collect these things, treat them the same. container model.


-->

## Midterm reflection (5-10 min)

Welcome to the second half of the semester!

Over the weekend, you wrote a reflection on your visual-rhetorical project; now, take a few minutes to write a broader reflection on the semester as a whole.

In the letter I wrote for the course syllabus, I asked you to think about "the affordances of digital media: that is, what’s made possible by working with bits instead of paper, even when we are still working with words? How do the answers change, or shift, as we move beyond words into aural and visual modes?"

<div class="alert alert-success">

<p>Please spend some time revisiting these questions, in writing, now that you've digitally crafted both sounds and images into coherent compositions. For example:
  <ul>
    <li>What's <em>afforded</em> (i.e. enabled, foregrounded, suggested) differently in these different media?</li>
    <li>What strategies carry across them?</li>
    <li>How do they extend or complicate your usual composition strategies in writing?</li>
  </ul>
</p>

<p>If you want, you could also consider how the particular software we used differs from other tools you might have employed toward similar ends: what's facilitated, and what's frustrated, by these tools, and how did that change your approach?
</p>
</div>

**Take 10 minutes.** I won't collect these directly today, but you will use them to develop your pitch for a collaborative project, and as a snapshot of your progress to look back on (and possibly quote) in a final reflection for the end of the course.

EXT: Reflect on your goals for the course: given your goals and expectations when you began this class, what have you begun to learn? Combined with what you now know about our projects and scheduling patterns, what would you give yourself as a goal for the rest of the term?

EXT 2: What do you expect the affordances of a website will be?

## 2. Web-design unit overview and assignment (10 min)

As I explained in the syllabus, your third project is to **build a responsive website using basic html and css files** — as opposed to a site manager like WordPress or Wix — **along with any media assets you wish to embed.** In assigning this, I have two main goals for you:

1. to learn how to manage a composite project made up of multiple interlinking files, and
2. to explore the affordances of the web design stack as a medium, and especially its ability to _flexibly render content for multiple audiences or reading priorities_.

<div class="alert alert-success">
To read the full assignment – and fork a copy for yourself – go to <strong><a href="https://github.com/benmiller314/website-portfolio-2019fall#project-3-website-portfolio">github.com/benmiller314/website-portfolio-2019fall</a></strong>.
</div>

Let's read through this together.

<!-- Go through overview, constraints, deadlines. -->

## 3. Markup: separating content from display (10-15 min)

| HTML | HyperText Markup Language |
| CSS | Cascading Style Sheets |

What does that mean??

Per [the tutorial I'm assigning you for homework](https://internetingishard.com/html-and-css/introduction#html-css-and-javascript),
> HTML is for adding meaning to raw content by marking it up.
CSS is for formatting that marked up content.

<!-- Make the connection to their own markup on the Issue Queue: bold, italic, etc. -->

In other words:

| HTML | HyperText Markup Language | structure (stays the same)|
| CSS | Cascading Style Sheets | display (can change) |


I'll start with a simple example: let's look at the code behind [getskeleton.com](http://getskeleton.com). I'll start with a right-click > inspect.

<!--
* head / body
* body has a big container
* inside the container is a section, a nav, and a bunch of divs (each with an id)
* open _typography_ div to show how the boxes just nest inside each other
-->

<details>
<summary>Now, let's change the display a bit...</summary>
<!-- implement one line at a time -->
<pre><code>
div {
  border: 1px dotted crimson;
  background-color: lightgray;
}
<!-- then mess with the color picker -->
</code>
</pre>
</details>

*Okay, but why do this in two separate steps? Why not just add those styles to the html directly?*

Because time-in-class is short, and because we have a wide range of web design experience among us, I'm going to accelerate past the beginning for a moment. In the process, we'll see examples of some of the essential things you can *do* with CSS – but we'll skip over the breadth of information you'd need to build something like this from scratch. My hope is that, having been to the top of the mountain, you'll have a better sense of why it's worth trekking across the desert of the tutorials to get back up there on your own two <del>feet</del> typing hands.

<div class="alert alert-info">
Come with me to the <a href="http://www.csszengarden.com">CSS Zen Garden</a>.
</div>

<!--
demo Garments,
Screen Filler,
A Robot Named Jimmy.

Emphasize that this is all _exactly_ the same html.
-->

## HW preview
Note that you can set Atom as your default text editor in GitHub Desktop, making it very easy to browse and edit all of a repo's files. I recommend it!

<figure>
<img src="{{site.github_url}}/uploads/gh-desktop--set-text-editor.png" alt="GitHub Desktop > preferences > advanced > external editor" />
<figcaption>Use the advanced tab in preferences</figcaption>
</figure>

## EXT: Start the homework tutorial.
I think the full tutorial's worth reading through, even if you're already familiar with the content (I was, and I still consolidated a lot of my understandings).

But if you're able to breeze through parts 1-4, and still have time left in class, please look through the web-related sections of the class  [Resources]({{site.github_url}}/resources) page, and click through to the documentation for anything that sounds interesting!

<!-- MOVED TO NEXT LESSON
## 4. "Web Design in 4 Minutes"... in 15 minutes


I expect this will take a bit more than four minutes, because I fully plan to interject, and I hope you will, too. But that's really what this is called:
[http://jgthms.com/web-design-in-4-minutes](http://jgthms.com/web-design-in-4-minutes/)
-->

## Homework for Next Time

* **Do** as much of the [Interneting is Hard (but it doesn't have to be)](http://web.archive.org/web/20190213013947/https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-4 (from "Introduction" through "Hello, CSS")
* **Show your work** by pushing your tutorial code to a repository
   - I've already created folders for parts 1-3 in the GH repo you just forked; clone it to your local computer, and you should be able to work in those folders and push.
   - Note that you'll need to add your own folder for part 4, and thereafter.
* **Bring** headphones for sonic isolation, if you want: we'll have some studio time next class.
