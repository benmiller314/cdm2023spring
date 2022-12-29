# Web Unit Studio / Deployment

**Work to have done**:

* [HTML/CSS tutorial](http://web.archive.org/web/20190213013947/https://internetingishard.com/html-and-css/) parts 1-6 or beyond
* Read up on [CSS selectors](https://css-tricks.com/how-css-selectors-work/) and relative specificity/priority
* Website proposal, posted to the [issue queue](https://github.com/pitt-cdm/miller2019spring/issues/12)

**Plan for the Day**:

1. Key steps (and a few options) in deploying via GitHub Pages (10 min)
2. In-browser testing: developer tools (10 min)
3. General notes re: proposals (5 min)
4. Studio (40-45 min)
5. HW Preview

## 1. Key steps (and a few options) in deploying via GitHub Pages (10 min)

* The most important file: index.html (or index.md)
* Three possible locations (root, branch, docs)
* Jekyll? Or hide?

## 2. In-browser testing: developer tools (10 min)

You can, in general, do worse than finding websites that you like and trying to figure out what they're doing that works.

But:
* minimalist designs don't always mean minimal markup
* *inspect*-ing a whole page can be daunting

Luckily, we have ways of dealing with that. First, most of the time we don't have to inspect a whole page – just the part of it we want to inspect more closely, whether to imitate or to adjust.

Yes, adjust. The inspector is especially helpful for testing new CSS rules. I'll just demo this briefly; you can play with it more as you work on your sites.

### Labeling invisible layout
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

And so on. (And then, when you see something positioned without using a div, you can inspect just that thing, and level up on layout.)

### Finding the perfect color
Not sure what color name (or hex) to use? Good thing there's a **color picker**! (Pro tip: to create high contrast, you can switch to HSL mode: that's Hue / Saturation / Luminosity. [Varying luminosity is the best way to get the contrast you want](http://www.eyequant.com/blog/hacking-web-design-with-neuroscience), most of the time.)

### Become a power-surfer
You can also use the inspector to hide something that's in my way (I do this all the time on websites that don't handle narrow widths well):
```css
nav {
    display: none;
}
```

### Or just test your designs - across devices
But it's also useful for testing out more permanent tweaks. Let's say I want to better differentiate headers on this site.

```css
h3 {
    font-style: italic;
    color: #00590c;
}
```

Or if I want to have something happen on hover, which a lot of you mentioned in your proposals.

```css
a:hover {
  background-color: #2ef96f;
}
```

## 3. General notes re: proposals (5 min)

* Hover will not work on a touch-screen-only interface, like a phone or tablet. <!-- Demo emulation mode -->

As a work-around, modify the rule to allow the same behavior on sustained click:

```css
a:hover, a:active {
  background-color: #2ef96f;
}
```

* If you're planning to include a lot of research, prepare a fallback possibility.

In designing this exercise, I'd been assuming that **the bulk of the work should be in the design and markup/coding**, and that you'd therefore be working primarily with pre-existing content. (This is why I called it a "website portfolio" in the original prompt.)

That said, I do want you to pursue your excitement. But be prepared for the possibility that you don't finish writing all your new content, if new content is what you're after. In that case, **it's good to know you have [lorem ipsum](https://loremipsum.io) available as a placeholder.** (And don't forget the [variants](https://loremipsum.io/#lorem-ipsum-all-the-things)...)


## Okay, now go to!

<div style="height:500px; height:50vh;">
<!-- This div left intentionally blank, for spacing -->
</div>


## Homework for Next Time

* **Do** more of the [tutorial](http://web.archive.org/web/20190213013947/https://internetingishard.com/html-and-css/), including at least Flexbox (8) and Responsive Design (10), if you haven't yet.
* **Compose and push** a website preview: a beginning.
    - If you're opting not to make this site public, make sure you can open it in a web browser from your Box... and that I have a link to the Box folder.
* Next class, we'll do our criteria generation. Consider: What shared baseline do you want to hold yourself to? What beyond that do you aspire to do, even if you don't quite succeed?
