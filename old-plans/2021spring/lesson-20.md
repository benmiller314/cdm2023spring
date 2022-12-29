
# Writer/Designer's studio: from structure toward layout

**Work to have done**:

* As much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as you can – at least parts 1-6 (from "Introduction" through "CSS Selectors") plus 8 ("Flexbox") and 10 ("Responsive Design") – as well as the Medium post on [Grid Layout](https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725) (and optionally [responsive grid](https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f))
* A first website preview, focused on content and structure (html)


**Plan for the day**:
1. Share and talk it out
2. Resources, some new
3. Set goals
4. Go forth! (Studio time or talk to me for demo / Q&A)
5. Revisit and update your goals
6. HW for next time

## 1. Share and talk it out (15 min)

In breakout rooms, share and discuss the previews you brought in for today... and talk through the questions and excitements that came up as you did it.

Write down any questions you'd like to bring to me in [the Google doc](http://bit.ly/cdm2021spring-notes)

EXT: I know some people are feeling behind, for various reasons. If you run out of previews to talk through in your group, but still have time left, continue in the tutorial assignments from where you left off – and add in my screencast video on Canvas (see below) after you finish with Flexbox.


## 2. Resources, some new (15 min)

I've been fielding a few questions by email since last class, and I expect you may have more now. Some things I think might help more than just the people I'm responding to:

### A screencast on `<div>`, repetition, and flexbox

Rather than take up class time on these things, which I do think are important, I recorded myself talking about ways to level up beyond the Flexbox tutorial; you can find that video [in the Panopto section on Canvas](https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9171fa85-be27-437d-99b9-acfa00f44a4f).

### When to use Grid, and when Flexbox?

Generally speaking, if you only have one dimension (one row, or one column), Flexbox is your friend. To put that another way: use [Grid for layout, Flexbox for components](https://ishadeed.com/article/grid-layout-flexbox-components/). (That link goes to a nice explanation, with examples, of when you'd want to use which.) Some things really are harder with Grid!

And remember that HTML is often about nesting boxes inside boxes: there's no reason you can't have a flexbox inside a gridbox.

### Do we *have* to use Grid or Flexbox?

Not at all! You can lay out your page using real widths and heights, and if you express them as responsive units (`em` or `%`), you'll even get scaling effects as the viewport changes size. To get a horizontal centering effect, you can use `margin: 0 auto;` on any block element with a declared width, or `text-align: center;` on any inline element, and you should be good to go.

That said, for dynamically adjusting space between elements, and especially for centering things vertically, these new layout tools are definitely your friends.

### Can I learn Flexbox in a more bloodthirsty way?

Try [Flexbox Zombies](https://flexboxzombies.com/), an interactive course that's currently free. In it, you imagine the flex layout as aiming a crossbow at undead monsters: you have to position the targets using CSS rules to survive. It's kind of slow-paced, but that's because it's filled with challenges for you to solve, with the idea being that typing out the rules many times will make them second-nature by the end.


## 3. Set goals for studio

What do you need to do to level up on HTML and CSS in the direction of your specific project? As usual, please write down some goals in the [google doc](http://bit.ly/cdm2021spring-notes#heading=h.twpohmiaq3vw), so I can get an overview of where everyone's at – and so you have a marker to come back to for your reflections, later.

<div class="alert alert-info">
Also for my sake and yours, please **be as specific as possible:** e.g. rather than “working on my site,” you might say, “choosing images for photo gallery” or “building grid for layout with top menu and areas for paragraphs with a featured image” etc etc.
</div>


## 4. Go forth!

I'll stay in the main room, for Q&A or demo purposes, but please do call me into a room if you need me!

Things I expect people have questions about include: grid layout, responsive design and media queries. But you let me know and I'll try to meet you wherever you are.

<div class="alert alert-warning">
As usual, to get credit for asynchronous participation, please add your intentions and exit notes to the google doc when you start and stop working – and aim to work for at least two 20-minute pomodoros.
</div>

Save about five minutes at the end to write me a brief exit note about what you've been working on.


## 5. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

<strong>Reply to your note in the <a href="http://bit.ly/cdm2021spring-notes#heading=h.twpohmiaq3vw">google doc</a>.</strong>
</div>

# Homework for next time

* **Continue** the [tutorial](https://internetingishard.com/html-and-css/) – or revisit the sections that are still confusing. I especially encourage you to look at the sections on [Semantic HTML](https://www.internetingishard.com/html-and-css/semantic-html/) ([Wayback version](https://web.archive.org/web/20201015230619/https://www.internetingishard.com/html-and-css/semantic-html/)) and [Web Typography](https://www.internetingishard.com/html-and-css/web-typography/) ([Wayback](https://web.archive.org/web/20201016104046/https://www.internetingishard.com/html-and-css/web-typography/)), and if you're having trouble with positioning even after looking at the resources I've shared, try reading the [Advanced Positioning](https://www.internetingishard.com/html-and-css/advanced-positioning/) ([Wayback](https://web.archive.org/web/20210213103939/https://www.internetingishard.com/html-and-css/advanced-positioning/)) section.
  - NB: I've been getting the Interneting Is Hard site to load in Chrome without Wayback, for whatever reason. Maybe I just have it cached.
  - Email me with any questions, noting that I can help fastest if you include a screenshot and a link. Better yet, [create a New Issue](https://github.com/benmiller314/cdm2021spring/issues/new/choose)! Then my answer to you can help others, too.
* **Compose and push** a second website preview, now adding or updating layout – or at least taking a stab at it, so you know what questions or concerns you'll have. A full draft of your website project is due in one week.
