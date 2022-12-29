---
layout: bottomnav
---

# Web Unit Workshop

**Work to have done**: a solid attempt at a complete website, ideally meeting baseline criteria. Rough edges are still welcome.

**Plan for the day**:

1. Workflow tweaks: still Describe -> Evaluate -> Suggest, but a wrinkle (5 min)
2. Evaluation reminder: our shared criteria (5 min)
3. Peer review workshop (3 times 10-12 min)
4. Evaluation revisited (10 min)
5. HW preview
6. EXT: Studio

<!-- SAVE FOR STUDIO
Two related goals:
* Lowest line-count challenge
  - does that div need to be there?
  - could those CSS rules be combined?
* Semanticity
  - can you tell what's going on just by reading the HTML file?
  - does the HTML hard-code any display (e.g. `<center>`, `<b>`) that should be in the CSS?  
-->

<div class="alert alert-warning">
<h2>#ThingsIShouldHaveToldYou</h2>
Your homepage should probably be called something like <strong>index.html</strong> (or index.md) for it to load automatically at the root directory of your website URL. If you're getting a 404 error when you open the root URL of your project, that might be the reason.
</div>

## Workflow Tweaks

As you remember from the sound and image units, I encourage you to **always start by describing** the piece, before judging what's good about it, so the creator knows whether you're on the same page. (Which is itself important feedback: _is my message getting through_.)

<div class="alert alert-white">
   <div class="alert alert-info">
      For this unit, in which display is a separate – and often challenging – concern, I'm going to ask you to use a <em>two-step description</em>.
   </div>

   <ol>
      <li><strong>First look at the HTML files, and say back what you see there.</strong> What seem to be the major content areas? What's given top-level focus? (e.g. what kind of thing gets its own page, or what's at &lt;h1&gt; status within a page?) What's next in the hierarchy?</li>
      <li>Once you've done that, <strong>turn to the browser and repeat the process for the display.</strong> What's given visual weight? What falls "above the fold"? Where are you invited to go next?</li>
   </ol>
</div>

From there, you can continue on to _evaluation_, using the shared criteria we developed on Thursday – and also the correspondence between the hierarchy you observed in the HTML and the hierarchy you observed in the rendered site.

<!-- NB: This is still a form of description: it's not about "good" or "bad" in the abstract but about where it meets or misses the shared or stated goals. -->

Finally, in your <em>suggestions</em>, some revision possibility that you think might help take the project to the next level: assume this is a work in progress. Given the goals, the focus, the criteria, what might be next? <!-- Pose this as a suggestion, not a command: and _interpret_ these as suggestions, not commands. -->

<!--
I have here to return to you the index cards from the visual unit – not from the comments you *received*, but the comments you *gave*. Read them over. **Were you doing describe/evaluate/suggest?** If so, be proud! See if you can do it again in a new sensory mode. If not, strive to level up today: train your attention to see before judging. -->

## 2. Evaluation reminder: our criteria (5 min)
We set up a few shared goals and constraints [bit.ly/cdm2019fall-criteria](https://docs.google.com/document/d/1NcXvQsBNPaumL6h_7ghKLJbQxPe_ALCiFMtPgaQI0Zk/edit#heading=h.z8d1igk08a86) to meet the baseline requirements. Let's try to help everyone get at least to there!

<aside>
<strong>Baseline criteria</strong>
For a minimum grade of B, all projects for this unit must:

<ul>
  <li>Use arrangement, size, color, visual rhythm, and/or contrast to focus viewers' attention</li>
  <li>Include at least three navigable html locations</li>
  <li>Have a clear mode of navigation among the locations (no dead ends)</li>
  <li>Include at least one css stylesheet</li>
  <li>Include at least one legally useable image, with alt text</li>
  <li>Successfully display in a local web browser</li>
</ul>

<strong>Aspirational inspirations</strong>
To target (but not guarantee) a grade above a B, the best projects for this unit may...

<ul>
  <li>Use Github Pages to load publicly over the Internet</li>
  <li>Use Jekyll-style html templates and variables, which can help minimize repetition</li>
  <li>If premade templates, try to change it and talk about what happened</li>
  <li>If not premade templates,
    <ul>
      <li>make it look clean and aesthetically modern (image-forward or minimalist)</li>
      <li>Use best practices for responsive design (e.g. @media queries to resize elements for mobile vs desktop viewing)</li>
      <li>Use best practices for accessible design (e.g. screen-reader-only navigation)</li>
    </ul>
  </li>
  <li>Incorporate Javascript interactivity or automation (carousel/slider, dynamic menus, etc)</li>
  <li>Use a consistent / considered color palette (and say why you chose it)</li>
  <li>Use imported (custom) fonts</li>
</ul>
</aside>

## 3. Peer Review Workshop (3 times 10-12 min)

Let's do this!

<div class="alert alert-success">
Before you leave your seat, <ol><li>load up your Atom project folder<sup>&#42;</sup>,</li><li>load your home page in a browser (preferably Firefox or Chrome), and</li><li>label <strong>three</strong> index cards <em>For: {yourname}</em>.</li></ol>
</div>

<sup>&#42;</sup> NB: if your site is dynamically generated from lots of files, e.g. with Jekyll or Flask, you may (also) want to open a View Source window in the browser to show the rendered HTML.


Then...

<div class="alert alert-success">
Go four seats clockwise around the room, hopefully arriving somewhere you haven't yet been for workshop. Label <em>one</em> index card <strong>From: {yourname}</strong>. View / read through the project fully at least once, then
<ol><li><strong>Describe</strong> what you see – first in the HTML, then in the browser –</li> <li><strong>Evaluate</strong> where it meets or misses the criteria,</li> and <li><strong>Suggest</strong> ways to meet and exceed the criteria!</li></ol>
</div>

I'll keep track of time.
<!-- first loop starts at 2:45 -->
<!-- second loop starts at 2:57 -->
<!-- third loop starts at 3:09 -->

On subsequent loops, note that **after** viewing the project first, you may also want to read and/or refer to the previous index cards.

## 4. Evaluation revisited (10 min)
Head back to your seats and take a minute to read **and photograph** the notes you've received. (Make sure your photos are legible; I'll be collecting the cards at the end of class.)

Based on your viewing, would anyone like to propose changes to the baseline criteria, or new aspirational goals to consider?


# Homework for Next Time
* Even as we zoom in toward the unit finale (again), I want to keep one eye open toward the bigger picture (again!). At this point, we have a number of [great ideas](https://github.com/benmiller314/cdm2019fall/issues/6) for [group projects](https://github.com/benmiller314/cdm2019fall/issues/10):
  - Collaborative soundscape narrative / podcast / radio show, perhaps traversing existing soundscape narratives
  - Art of Foley (adding sounds to video - maybe one of [these](https://www.google.com/search?q=short+videos+no+sound&tbm=vid&sxsrf=ACYBGNTjlnYAR93lkuo0q2cwvLs06VgiNw:1572973957460&source=lnt&tbs=dur:s&sa=X&ved=0ahUKEwiyn-bPyNPlAhUOyFkKHZIRDisQpwUIIQ&biw=1440&bih=798&dpr=1))
  - "Reverse-Foley" (visually animating, or filming, a soundscape)
  - Digital stop-motion / flip-book animation ([several tools](https://www.freelancer.com/articles/graphic-design/best-free-animation-software) available)
  - Animated or text-based game (perhaps using [Twine](http://twinery.org/))
  - Visual programming (probably in [Scratch](https://scratch.mit.edu/about))
  - UI/UX design in Adobe Suite (talk to [Margaret](mailto:mpalko@pitt.edu) about this one!)

* Skim through any links above that seem intriguing, and if something strikes you, **[post a proposal]({{site.github.issues_url}}/13) to try to recruit partners**. As before, there is no minimum length for these posts.

* Next class will be a web designers' studio: **optionally bring headphones for [sonic isolation](http://noisli.com)**, and whatever else you need to work towards finalizing your website portfolio.
  - The final draft is due at the end of the day on Sunday, and a reflection by class-time on Tuesday; see the [prompt](https://github.com/benmiller314/webste-portfolio-2019fall#project-3-website-portfolio) for further details.



## EXT:
If any time remains, go ahead and get started on those revisions!
