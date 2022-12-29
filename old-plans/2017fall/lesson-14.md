## Backstage on the Web; Building on Others' Designs

**Texts to have read**:

* *Writer/Designer* chapters 2 and 3, on "Analyzing Multimodal Projects" and "Choosing a Genre and Pitching Your Project."

**Work to have done**:

* Analyzing a website's design choices (posted to reflections category on WordPress)


<!--
[toc tag="h2" title="Plan for the Day"]
-->

### Insights from reflecting on websites' design choices (10 min)

* we like clothes
* the current moment is very image-forward, with minimal text
* alignment and whitespace are used to group things more than borders or dividers
* sans-serif more common for body fonts, serif sometimes for headings

While prepping for class, I found some interesting [data from an eye-tracking firm](http://www.eyequant.com/blog/hacking-web-design-with-neuroscience) that's relevant here. I'll summarize-skim, leaving the link for you to peruse in more depth, but here's their big take-away:
[!The Attention Hacker's Checklist, from eyequant.com](https://www.eyequant.com/hs-fs/hubfs/Checklist-EQ.png?t=1508348609531&width=605&height=528&name=Checklist-EQ.png)

What does that help you see about the sites you studied for today?

### Using your browser's inspector (10 min)
Two more big insights from the homework due today:

* minimalist designs don't always mean minimal markup
* *inspect*-ing a whole page can be daunting

Luckily, we have ways of dealing with that. First, most of the time we don't have to inspect a whole page – just the part of it we want to inspect more closely, whether to imitate or to adjust.

Yes, adjust. The inspector is especially helpful for testing new CSS rules. I'll just demo this briefly; you can play with it more as you work your way through the tutorials.

For instance: if I wanted to see where all the divs on the site were, I could temporarily put a border on them all:
```css
div {
    border: 1px #333 solid;
}
```

I could go further and see how they drill down. This will highlight all divs that are the direct child of another div:
```css
div > div  {
  background-color: greenyellow;
}
```
<!-- FOR NEXT TIME: don't forget to show the color picker! -->

And so on. (And then, when you see something positioned without using a div, you can inspect just that thing, and level up.)

Or I could hide something that's in my way (I do this all the time on websites that don't handle narrow widths well):
```css
nav {
    display: none;
}
```

But it's also useful for testing out more permanent tweaks. I want to fix indented bullets on this site, for example, so they don't look the same as the top-level bullets.
```css
.entry-content ul li ul li {
    list-style-type: circle;
}
```


EXT: If time allows, it's worth looking more closely at [how CSS selectors work](https://css-tricks.com/how-css-selectors-work/) – especially [when two rules collide](https://css-tricks.com/specifics-on-css-specificity/). With classes and ids, you can get a lot more specific than html elements! (And you'll usually need to.)


### More brainstorming, and hand-drawn site sketches (20 min)
Before we get into the weeds of finding the html that will execute our vision for a site – a process which can often produce the distracting kinds of difficulty – it can be useful to get a sense of how we would ideally *want* to organize our site. We're going to do a little drawing, but first, a little reflective writing.

1. Take out, if you have them, your notes from last time about possible project pitches. If you don't, or if you're inclined to do so, **take a minute or two to brainstorm again**: (2 min) <blockquote>What have you begun to learn, and what, especially, haven't you begun to learn? What skills do you want to have practiced before the semester is over? Can you think of any projects you might compose over the next month or so that would help you get that practice?</blockquote>
2. Choose one of these skills or projects to work with for now. Mark it in some way. Then ask yourself: **What are all the parts of this?** What steps, or pieces, or roles, are involved? **Make a quick list, without diving into any one item.** (2 min)
3. I'm going to interrupt you now and ask you to set aside the list, just for now, and ask: **What's the heart of this?** What's the essential component? What's the value proposition for your classmates to join you in this project? Write down whatever comes. (2 min)
4. Okay. So whether that worked or not, you should now have at least a small list of things that could belong in your web-based pitch. Given what's essential, and given the principles of designing for attention we learned earlier, make a quick sketch of a website's landing page. (5-10 min)
 * Not sure what that should look like? Here are [33 examples](http://designbeep.com/2012/05/17/33-great-examples-of-web-design-sketches/) (but no one is asking you to be as elaborate as the most elaborate of these)
 * EXT: Finished one drawing? Make another, using a different system of visually organizing your information.
 * Personal tip: I find it useful to divide the horizontal space into 12, so I can easily use [Bootstrap CSS's grid system](https://getbootstrap.com/docs/4.0/layout/grid/). Here, then, is one more example: <img src="{{site.base_url}}/assets/img/ben-sketches-for-web-design-assignment-website.jpg" alt="Ben's sketches for the web-design assignment's web design">.



### Self-paced exploration
<div class="alert alert-success">
**Read and follow along with the tutorial disproving the claim that <a href="https://internetingishard.com/html-and-css/">"html & css is hard"</a>.** Actually make the files the tutorial suggests; at the end of class, you can commit your files and push to GitHub.

NB: the lab computers don't have Atom, but they do have SublimeText, which is very similar.
</div>

EXT/ALT: If you're good on what a CSS class is, and how to add it to an HTML element, read up on [Bootstrap](https://getbootstrap.com/), a very widely used CSS framework. What that essentially means is that they've pre-created a bunch of CSS classes for you, so you can start using them to design your own layout from scratch. It's a little like Lego for web design, only free.


### Before you leave
I want to show you where/how to turn a github repo with html files into an actual website. All you need is an index.html file in the home directory, and to activate GitHub Pages:

[!screencast: activating github pages from the settings page](activate-github-pages.gif)

<!--
* in-class writing: hand-drawn site mockups, inspired by
* Self-paced lessons on ["html & css is hard"](https://internetingishard.com/html-and-css/)
* EXTs / bonus features on
 - using browser inspector;
 - CSS frameworks (Bootstrap);
 - Responsive templates (html5up, templated.co)
 - how to publish a working website using github.io
-->




## Homework for next time
**Inputs**:

* Continue reading and following along with the tutorial disproving the claim that ["html & css is hard"](https://internetingishard.com/html-and-css/). Spend at least an hour, aiming to learn something you don't already know.
 - If this is *all* familiar, including responsive design, read up on accessibility and "universal" design, starting here: [Introduction to Web Accessibility](https://webaim.org/intro/).
* Once you know what `<img>` tags are, review this guidance on how and why to include the alt attribute in all of your `<img>` tags: [webaim.org/techniques/alttext/](https://webaim.org/techniques/alttext/)

**Outputs**:

* Come in ready to ask questions of your groupmates.
* **Push a draft website to github**; it's fine for now if all you have to post is your tutorial progress. By next Thursday, 10/26, though, I'll ask for real drafts.

**Administrative**:

* That date reflects an update since Tuesday; I've pushed everything back by one lesson, to make sure we have time to get up to speed and gather criteria.
* If you haven't yet, sign up for a midterm conference with Ben over the next two weeks (absolute latest deadline: 11/9)
