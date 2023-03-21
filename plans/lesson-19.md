# Web Unit Studio / Layout Q & A

**Work to have done**:

* Kevin Powell's video on [5 simple tips to making responsive layouts the easy way](https://www.youtube.com/watch?v=VQraviuwbzU&list=PL4-IK0AVhVjM6kuUoUexfmnD8vHtZkXdd&index=4)
* As much of the [Interneting is Hard](https://internetingishard.com/html-and-css/) tutorial as you can, including at least parts 1-6 (from "Introduction" through "CSS Selectors") plus 8 ("Flexbox") and 10 ("Responsive Design")
* Readings on [Grid Layout](https://medium.com/deemaze-software/css-grid-layout-crossed-sections-fca9e956e725) (and optionally the followup post on [responsive grid](https://medium.com/deemaze-software/css-grid-responsive-layouts-and-components-eee1badd5a2f)).
* A website preview: just get something started, not necessarily with layout

**Plan for the day**:

1. CSS layout example: grid areas
  * And some FAQs on Grid and Flex
2. Studio: toward a laid-out preview
  * Set Goals
  * Go forth!
  * Exit note




## 1. CSS layout example: Grid Areas

In the EXT readings on CSS Grid, from over the weekend, I'd mentioned [Grid By Example](https://gridbyexample.com/learn), but I suspect not many people made it that far. I'd like to play around with one of the CodePens from that site (by web developer Rachel Andrew), as a way of giving you some examples of what Grid offers in terms of layout.

I'll be in her [Grid by Example 11: Defining Grid Areas](https://codepen.io/rachelandrew/pen/oXKgoQ?editors=1100), which is a CodePen.

<!-- Points to hit:

* We can easily stretch the header or the sidebar
* grid-template-columns: repeat(3, 120px);
* grid-template-columns: 120px 1fr;
* We can make the Content area its own grid (though NB that it's helpful to exclude the title of the section, so we'd need a wrapper)
* grid-template-columns: repeat(autofit, 120px)
  grid-template-rows: minmax(120px, max-content)

-->


### FAQ on layout

<details><summary>When to use Grid, and when Flexbox?</summary>

<p>Generally speaking, if you only have one dimension (one row, or one column), Flexbox is your friend. To put that another way: use <a href="https://ishadeed.com/article/grid-layout-flexbox-components/">Grid for layout, Flexbox for components</a>. (That link goes to a nice explanation, with examples, of when you'd want to use which.) Some things really are harder with Grid!</p>

<p>And remember that HTML is often about nesting boxes inside boxes: there's no reason you can't have a flexbox inside a gridbox.</p>
</details>

<details><summary>Do we <em>have</em> to use Grid or Flexbox?</summary>

<p>Not at all! That said, I do recommend expressing widths and heights through responsive units (<code>em</code>, <code>rem</code>, <code>%</code>, <code>vh</code>, and <code>vw</code>) or via <code>min-</code> and <code>max-</code> rules, rather than in absolute terms. As Powell explained, this means you'll get scaling effects as the viewport changes size. To get a horizontal centering effect, you can usually use <code>margin: 0 auto;</code> on any block element with a declared width, or <code>text-align: center;</code> on any inline element, and you should be good to go.</p>

<p>That said, for dynamically adjusting space between elements, and especially for centering things vertically, these new layout tools are definitely your friends.</p>
</details>

<details><summary>Can I learn Flexbox in a more bloodthirsty way?</summary>

<p>Try <a href="https://flexboxzombies.com/">Flexbox Zombies</a>, an interactive course that's currently free. In it, you imagine the flex layout as aiming a crossbow at undead monsters: you have to position the targets using CSS rules to survive. It's kind of slow-paced, but that's because it's filled with challenges for you to solve, with the idea being that typing out the rules many times will make them second-nature by the end.</p>
</details>


## 3. Studio: toward a full working draft

Keep working on your projects and/or tutorials, knowing that you have a draft due by Tuesday morning. See if you can get up to [baseline](https://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.5bpexk6at73l)! (In general, use the gdoc as your source for the most up-to-date baseline, since it also has clarifying commentary.)

I'm hoping by now you're starting to get a feel for how to use the browser's inspector to see what's being rendered, and how!

And now you know that includes layout like grid and flex containers, too!


### Set Goals

What do you need to do to level up on HTML and CSS in the direction of your specific project? As usual, please write down some goals in the [shared google doc](https://bit.ly/cdm{{site.course.slugterm}}-notes), **set a goal for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project?

<div class="alert alert-info">
Also for my sake and yours, please <strong>be as specific as possible:</strong> e.g. rather than “working on my site,” you might say, “choosing images for photo gallery” or “building grid for layout with top menu and featured image” etc etc.
</div>

*Not sure where to start?*
  - Check [Web Design in 4 minutes](http://jgthms.com/web-design-in-4-minutes) and at least add spacing and some web-ready fonts.
  - I also have a [7-minute screencast building on the end of that Flexbox tutorial](https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9171fa85-be27-437d-99b9-acfa00f44a4f) with some tips on cleaning up and proofreading your code. Hopefully informative? (Apparently I bumped against the microphone toward the beginning -- terribly sorry for the occasional scraping noise!)

*Already feeling done?* Ask yourself:
  - Are you repeating the same CSS rule in multiple places? Instead, see if you can reuse CSS classes in multiple places, extending them where you need to.
  - Does that div need to be there? If it's not for layout or semantic grouping, it might not be necessary. See that screencast above for an example.
  - Do you have style or presentation directly in the HTML? See if you can extract it out to the stylesheet.
  - Want more relative values for things like color? See [css-tricks.com/a-complete-guide-to-custom-properties/](https://css-tricks.com/a-complete-guide-to-custom-properties/).




### Go forth! And Don't forget to document your process

<div class="alert alert-success">
Don't forget to save periodically as you go:
 <ul>
   <li>as a project file</li>
   <li>as a screenshot, showing your process</li>
   <li>as a git commit, saying what you've just achieved</li>
 </ul>
</div>

### Exit note

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet? Work through a tutorial or two (and which)?

<strong>Reply to your note in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">google doc</a>.</strong>

## Homework for next time

* **Continue** the [HTML &amp; CSS tutorial](https://internetingishard.com/html-and-css/), adding at least Semantic HTML (12) and Web Typography (14). If you're encountering weird layout intransigence, you may also want to try Advanced Positioning (9).
  - Remember that the main tools for layout now in use are Grid and Flex; you can probably skip the chapter on Float except for particular use-cases (e.g. text that wraps around an image).
  - **Email me with any questions**, noting that I can help fastest if you include screenshots and links to your site/repo. Better yet, [create a New Issue]({{site.github.issues_url}}/new/choose)! Then my answer to you can help others, too.
* **Compose and push** a second website preview, now adding or updating layout. A full, workshop-ready draft of your website project is due in one week.