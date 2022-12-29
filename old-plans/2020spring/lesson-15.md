
# Midterm Reflections and Intro to Markup

**Work to have done**:

* Your final-for-now Visual Rhetorical Collage and Reflection
* Download and install the [Atom text editor](http://atom.io)

**Plan for the day**:

1. Midterm reflection (5-10 min)
2. Share and discuss reflections (5-10 min)
3. Introduction to markup languages (15-20 min)
4. Web-design unit overview and assignment (10 min)
5. CSS in 4 minutes (10-15 min)
6. Homework preview

<!-- NOTE FROM LAST TIME: don't cut CSS in 4 minutes, and maybe even start with it? I ended up with 30 minutes left!!

cdm2020spring update: NOPE, REVERT NOTE FOR NEXT TIME from last time: we ran out of time for CSS in 4 minutes (code pen, y'all), and it's probably a better use of time to **get everyone into the tutorial so you can troubleshoot Atom with them.** In fact, skip it until after they've seen the CSS selectors tutorial!

-->

## Midterm reflection (8-10 min)

Welcome to the second half of the semester!

Over the weekend, you wrote a reflection on your visual-rhetorical project; now, take a few minutes to write a broader reflection on the semester as a whole.

In the letter I wrote for the course syllabus, I asked you to think about "the affordances of digital media: that is, what’s made possible by working with bits instead of paper, even when we are still working with words[...] How do the answers change, or shift, as we move beyond words into aural and visual modes?"

<div class="alert alert-success">

<p>Please spend 8-10 minutes revisiting these questions, in writing, now that you've digitally crafted both sounds and images into coherent compositions. For example:
  <ul>
    <li>What's <em>afforded</em> (i.e. enabled, foregrounded, suggested) differently in these different media?</li>
    <li>What strategies carry across them?</li>
    <li>How do they extend or complicate your usual composition strategies in writing?</li>
  </ul>
</p>

<p>If you want, you could also consider how the particular software we used differs from other tools you might have employed toward similar ends: what's facilitated, and what's frustrated, by these tools, and how did that change your approach?
</p>
</div>

**I won't collect these directly, but I will ask for volunteers to share as part of a discussion in today's class.** You should also keep them to help you develop your pitch for a collaborative project, and as a snapshot of your progress to look back on (and possibly quote) in a final reflection for the end of the course.

EXT: Reflect on your goals for the course: given your goals and expectations when you began this class, what have you begun to learn? Combined with what you now know about our projects and scheduling patterns, what would you give yourself as a goal for the rest of the term?

EXT 2: What do you expect the affordances of a website will be?

## 2. Share and discuss reflections (5-10 min)

Any volunteers to share?

Anyone have a different response?


## 3. Introduction to Markup Languages (10-15 min)

### Begin with a breath
Our next unit takes us into the world of hypertext, a more interactive medium. Before we dive in deep, <strong>come with me to the <a href="http://www.csszengarden.com">CSS Zen Garden</a></strong>.

Some things to notice:

* Responsive design: the same page can change appearance to suit the "viewscreen" (especially as the width changes).

<!-- demo Verde Moderna (the default), -->

* The visual hierarchy holds here, too – including uses of negative space as a way of establishing rhythm.

<!-- Screen Filler, -->

* So, too, are we retaining the importance of color schemes for both coherence and contrast.

<!-- Mid-Century Modern -->

* This is all _exactly_ the same html.

<!-- Even A Robot Named Jimmy. -->

### Markup: separating content from display
How?

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>acronym</th>
      <th>stands for</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML</td>
      <td>HyperText Markup Language</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>Cascading Style Sheets</td>
    </tr>
  </tbody>
</table>

What does that mean??

Per [the tutorial I'm assigning you for homework](https://internetingishard.com/html-and-css/introduction#html-css-and-javascript),
> HTML is for adding meaning to raw content by marking it up.
CSS is for formatting that marked up content.

<!-- Make the connection to their own markup on the Issue Queue: bold, italic, etc. Make the connection to -->

In other words:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>acronym</th>
      <th>stands for</th>
      <th>used for</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML</td>
      <td>HyperText Markup Language</td>
      <td>content, groupings</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>Cascading Style Sheets</td>
      <td>display / presentation</td>
    </tr>
  </tbody>
</table>

There are other languages that interact with these two, especially JavaScript, but also PHP and Python and Ruby: they can dynamically generate or change the HTML and CSS. And there are preprocessor languages that make it easier to generate HTML and CSS on your own: Markdown, the syntax you use in GitHub READMEs and forum posts, is essentially a shortcut form of HTML. But HTML and CSS are the core of what gets shown on the screen.

Let's take Markdown as an example:

* If you want to make something bold, you...
  - put `**asterisks**` on either side of it.
* If you want italics, you...
  - put `_underscore_` on either side (single asterisks will work, too).

<div class="alert alert-info">
The basic idea is that you need to signal where the <em>marked-up text</em> begins and ends.
</div>

The same is true in HTML, but it looks a little different:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>what we’re marking</th>
      <th>Markdown syntax</th>
      <th>HTML syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>strong text</td>
      <td><code class="language-plaintext highlighter-rouge">**surrounding asterisks**</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;strong&gt;opening and closing tags&lt;/strong&gt;</code></td>
    </tr>
    <tr>
      <td>emphasized text</td>
      <td><code class="language-plaintext highlighter-rouge">_surrounding underscore_</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;em&gt;opening and closing tags&lt;/em&gt;</code></td>
    </tr>
  </tbody>
</table>

<div class="alert alert-info">
<p>Unlike in Markdown, opening and closing tags in HTML aren't exactly the same. But they're <em>almost</em> the same: a closing tag in HTML just adds the slash after the first angle bracket.</p>

<p>You can think of them as being like <a href="https://xkcd.com/859/">parentheses</a>: In general, every HTML tag you open should close. (You can nest a complete pair of tags inside another pair (like these parentheses), but you can't close the outer pair before closing the inner pair without causing problems.)</p>
</div>

One nice thing about having the tags themselves marked by angle brackets is that you can add information to them:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>what we’re marking</th>
      <th>Markdown syntax</th>
      <th>HTML syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>a basic hyperlink</td>
      <td><code class="language-plaintext highlighter-rouge">[anchor text](http://destination)</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination"&gt;anchor text&lt;/a&gt;</code></td>
    </tr>
    <tr>
      <td>a hyperlink with extra info</td>
      <td><em>no default way to do it!</em></td>
      <td><span title="title text is what you see on hover"><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination" class="dummylink external" title="Explanation of where link goes"&gt;anchor text&lt;/a&gt;</code></span></td>
    </tr>
  </tbody>
</table>

### A Demo
Some of this is easier to understand with a live demo! Let's head over to a [CodePen](https://codepen.io/benmiller314/pen/poJROZM?editors=1100) where we can get some instant results from adding new HTML and CSS rules.

<!--
CSS rules to hit:
1. headers
2. paragraphs
3. using Atom to auto-close tags
4. no default spacing: let's change it!
5. a div is like a layer-group: collect these things, operate on them together. it's a container.
6. ids and # selectors
7. classes and . selectors
 -->

## 4. Web-design unit overview and assignment (10 min)

As I explained in the syllabus, your third project is to **build a portfolio website using basic html and css files** — as opposed to a site manager like WordPress or Wix — **along with any media assets you wish to embed.** In assigning this, I have two main goals for you:

1. to learn how to manage a composite project made up of multiple interlinking files, and
2. to explore the affordances of the web design stack as a medium, and especially its ability to _flexibly render content for multiple audiences or reading priorities_.

<div class="alert alert-success">
To read the full assignment – and fork a copy for yourself – go to <strong><a href="https://github.com/benmiller314/website-portfolio-2020spring#project-3-website-portfolio">github.com/benmiller314/website-portfolio-2020spring</a></strong>.
</div>

Let's read through this together.

<!-- Go through overview, constraints, deadlines. -->

## 5. "Web Design in 4 Minutes"... in 15 minutes
<!-- Okay, revert NOTE FOR NEXT TIME from last time: we ran out of time for this, and it's probably a better use of time to get everyone into the tutorial so you can troubleshoot Atom with them. In fact, skip it until after they've seen the CSS selectors tutorial! -->

I expect this will take a bit more than four minutes, because I fully plan to interject, and I hope you will, too. But that's really what this is called:
[http://jgthms.com/web-design-in-4-minutes](http://jgthms.com/web-design-in-4-minutes/)



## Homework for Next Time

* **Do** as much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-4 (from "Introduction" through "Hello, CSS")
* **Show your work** by pushing your tutorial code to a repository
   - I've already created folders for parts 1-3 in the GH repo you just forked; clone it to your local computer, and you should be able to work in those folders and push.
   - Note that _you'll need to add your own folder_ for part 4, and thereafter.
* **Bring** headphones for sonic isolation, if you want: we'll have some studio time next class.
