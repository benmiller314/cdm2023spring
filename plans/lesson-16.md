
# Intro to Markup and Web Design

**Work to have done**: Write a website proposal and post it to the <a href="{{site.github.issues_url}}">issue queue</a>

**Plan for the day**:

1. Introduction to markup and style
2. Brief tour of key VSCode features (and key extensions)
3. Start the tutorial (with chapter 2)
4. EXT: Tour of unit resources
5. HW for next time


<aside>
<p>A quick note about your proposals: First, I'm excited to see how many great ideas you have! If you haven't yet posted and want to talk to me, please email or come to office hours. And don't forget about those parachute prompt options...</p>

<p>Second: I want to warn you about the risks of scope creep. If you're still learning HTML and CSS, <em>you probably want to limit how much new material you need to actively research or compose.</em> Instead, <strong>plan around a minimum deliverable product</strong>, with stretch goals on top of that. For example, could you create a mockup with <a href="https://loremipsum.io/">Lorem Ipsum</a> (placeholder) text and images, and then work on replacing it if time allows? Could you try writing just one or two blog posts at first, but build space for where more will go?</p>

</aside>



## 1. Introduction to markup and style

### Begin in the garden
Before we dive in deep, <strong>come with me to the <a href="http://www.csszengarden.com">CSS Zen Garden</a></strong>.

Some things to notice:


* Responsive design: the same page can change appearance to suit the "viewscreen" (especially as the width changes).

<!-- demo Verde Moderna (the default), -->

* The visual hierarchy holds here, too – including uses of containment and alignment to form groups, and negative space to establish rhythm.

<!-- Screen Filler, -->

* So, too, are we retaining the importance of color schemes for both coherence and contrast.

<!-- Mid-Century Modern -->

* Oh, and also? Every page you've just seen has _exactly_ the same underlying content: literally the same HTML file.

<!-- Even A Robot Named Jimmy. -->

### HTML vs CSS: separating content from display
How? The key is encoding the content separately from the presentation. And that's where our "web stack" begins: with HTML and CSS.

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

In other words, per [the tutorial I'm assigning you for homework](https://www.internetingishard.com/html-and-css/introduction/#html-css-and-javascript),

<blockquote class="blockquote">
    <ul><li>HTML is for adding meaning to raw content by marking it up.</li><li>CSS is for formatting that marked up content.</li></ul>
</blockquote>


There are other languages that interact with these two, especially JavaScript, but also PHP and Python and Ruby: they can dynamically generate or change the HTML and CSS. There are also "preprocessor" languages that make it easier to write HTML and CSS in the first place by eliminating some repetition. You've already seen one of these: Markdown, the syntax you use in GitHub READMEs and forum posts, is essentially a shortcut form of HTML.

But even with all that complexity, it boils down to this: HTML and CSS are the core of what gets shown on the screen.

### HTML gives the document *structure*
Even if you've never used a formal markup language, you already use symbols to highlight one part of a text document and show that it's different from the rest. Let's take Markdown as an example:

* If you want to make something **bold**, you...
  - put `**asterisks**` on either side of it.
* If you want _italics_, you...
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
      <th title="By default. In practice, you can use CSS to change &lt;em&gt; to red text, or a different font, etc, instead of italics – and so on for any element.">What you get<sup>*</sup></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>strong text</td>
      <td><code class="language-plaintext highlighter-rouge">**surrounding asterisks**</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;strong&gt;opening and closing tags&lt;/strong&gt;</code></td>
      <td><strong>strong text</strong></td>
    </tr>
    <tr>
      <td>emphasized text</td>
      <td><code class="language-plaintext highlighter-rouge">_surrounding underscore_</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;em&gt;opening and closing tags&lt;/em&gt;</code></td>
      <td><em>emphasized text</em></td>
    </tr>
  </tbody>
</table>

<div class="alert alert-info">
<p>Unlike in Markdown, opening and closing tags in HTML aren't exactly the same. But they're <em>almost</em> the same: a <strong>closing tag</strong> in HTML just adds the slash after the first angle bracket.</p>

<p>You can think of them as being like <a href="https://xkcd.com/859/">parentheses</a>: In general, <strong>every HTML tag you open, you should close.</strong> (You can nest a complete pair of tags inside another pair (like these parentheses), but you can't close the outer pair before closing the inner pair – at least, not without causing problems.)</p>
</div>

<!-- <aside class="alert alert-white">
Pro tip: Atom can automatically close the most recently opened tag. See Packages &gt; Bracket Matcher &gt; Close Current Tag, where you should also find a keyboard shortcut like <code>Cmd+Option+.</code>. (The shortcut's way more convenient, I find.) I like to use this also as a form of proofreading: it reassures me that any tags still open are what I expect is still open.</aside> -->

One nice thing about having the tags themselves marked by angle brackets is that you can add information to them, called <em>parameters</em>:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>what we’re marking</th>
      <th>Markdown syntax</th>
      <th>HTML syntax</th>
      <th>what you get</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>a basic hyperlink</td>
      <td><code class="language-plaintext highlighter-rouge">[anchor text](http://destination)</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination"&gt;anchor text&lt;/a&gt;</code></td>
      <td><a href="http://destination">anchor text</a></td>
    </tr>
    <tr>
      <td>a hyperlink with extra info</td>
      <td><em>no default way to do it!</em></td>
      <td><span title="title text is what you see on hover"><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination" title="Explanation of where link goes"&gt;anchor text&lt;/a&gt;</code></span></td>
      <td><a href="http://destination"  title="Explanation of where link goes">anchor text</a></td>
    </tr>
  </tbody>
</table>

### HTML in practice

Armed with that information, you now know enough to go back to the [CSS Zen Garden](http://www.csszengarden.com/) and see how it's structured.

Right-click in any blank spot on the page, and choose **View Source** from the context menu that pops up.

Let's have a look!

<div class="alert alert-warning"><p>NB: Chrome and Firefox have the best tools for web development, as we'll see. If you're using Safari, you won't see View Source by default. But you can <a href="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html">activate it under Safari &gt; Preferences &gt; Advanced</a>, down on the bottom: "Show Develop menu in menu bar."</p>

<details><summary>Show me</summary>
<figure><img src="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/Art/00developmenu_2x.png" alt="screenshot of Safari advanced preferences page" /></figure>
</details>

<p>While you're there, you may want to tell the Smart Search Field to <a href="https://apple.stackexchange.com/questions/371473/always-show-full-url-in-safari-address-bar">show the full site address</a>, too. URLs often contain a lot more useful info than just the home page!</p>

</div>

<details><summary>A few things to note in the Zen Garden source</summary>
<ul class="spaced">
<li><code>h1</code>, <code>h2</code>, and <code>h3</code> are headers, and establish <em>hierarchy</em>, and can be used to generate a page outline. You shouldn't skip levels.</li>
<li><code>p</code> is a paragraph.</li>
<li><code>a</code>, as we saw above, is an anchor for a hyperlink; it almost always has a <em>hypertext reference</em>, or <code>href</code>, as a parameter inside the opening tag.</li>
<li><code>div</code>s are like layer groups: they wrap around content that function as a unit.</li>
<li><code>section</code>s and <code>header</code>s and <code>footer</code>s are basically special <code>div</code>s!</li>
<li><code>class</code>es and <code>id</code>s are <em>labels</em> we can use to identify reusable content-types (classes) or unique locations (ids) within the document. They live as parameters inside opening tags.</li>
</ul>
</details>

### CSS in practice

**CSS functions by _selecting_ labeled content** – HTML elements or classes, and sometimes other contextual cues – **and assigning _rules_** for how to display what's been selected.

These rules generally live in a _style sheet_ that's linked inside the `head` element of the HTML document.

To see this in action, let's look at [the stylesheet I'm using for this site]({{site.github_url}}/assets/css/screen.css)!


### You can play

You can View Source on literally any website -- though some are more complicated than others.

You can also Inspect a live website, using the same context menu (again, Safari users have this disabled by default), and see all the CSS rules currently being applied to any HTML element you want.

What's more, you can *change or add* CSS rules on the fly. (It'll stay as long as you don't refresh the page... though you can also copy the new rules before you leave.)

You'll want to come back to this when you're working on your own designs!

<!-- If that's too much, we could go back to the [codepen](https://codepen.io/benmiller314/pen/poJROZM), using the examples from the tutorial's Introduction and modifying from there. -->


## VS Code orientation, then start the homework tutorial

For now, though, I suspect for many of you it'll be most useful to get your feet back on the ground.

I'll be asking you to work through the tutorials at [Interneting is Hard (but it doesn't have to be)](https://www.internetingishard.com), starting over break with at least the first four chapters: that will take you from "what is HTML?" through "Hello, CSS!"

<div class="alert alert-success"><p>Before you leave today, I want to make sure you're able to get up and running with your text editor and a browser, and seeing how they interact.</p></div>

The first chapter of the tutorial ("Introduction") mostly covers what we just talked about, and – unlike every other chapter – doesn't include any hands-on code examples that you're supposed to copy. So for today's class, I'd like you to **start with chapter two: "[Basic Web Pages](https://www.internetingishard.com/html-and-css/basic-web-pages/)"**.


### Key VS Code features that will make your life easier

If you haven't yet done so, clone your forked repository onto your local computer, and open it up: GitHub Desktop should even give you the option to do so directly in your text editor of choice. 

<figure><img src="../assets/img/github-desktop--open-in-vscode.png" alt="GH Desktop's open in editor button appears when there are no changes to commit.'" />
</figure>

If at any time you need to open the files from VS Code directly, you can also open the explorer from the sidebar, and choose your root folder from there.

<figure><img src="../assets/img/vscode--open-folder.png" alt="VS Code's open folder button appears in the explorer when you haven't yet specified your workspace.'" style="max-height:40vh" />
</figure>

NB: If you're using another text editor, look for ways your editor can do these things, too!


<!-- NOTES FROM 2022 SPRING:
* Demo with the webs assignment repo, not your lesson plan. *Show* the tutorials folder and its subfolders.
* Right-click the sidebar to create a new file/folder
* Right-click the sidebar to Show in Finder, double-click to open in your web browser. (How did you not have this?!)
* SKIP THE REST – newbies don't need to know about the shortcuts yet, oldbies (oldbies??) don't need to be told – and you've been talking for 45 minutes already. 

 -->

* Create new files and folders within the explorer (right-click on a blank space)

* Right-click in the explorer to Reveal a file in Finder/Explorer. From there, you can double-click to open an html file in your browser.

* Split Left / Split Right (right-click any filename)
  - View your HTML and CSS files at the same time! Or any two files. Or three, or six if you want to split top/bottom, too. It's the best.


<!-- * Comment out current line (Edit > Toggle Comment or the more-convenient keyboard shortcut: look in your menu) -->

 

### Okay, go ahead and do chapter 2!

NB: I've already created folders for parts 1-3 in the GH repo you just forked and cloned, so you should be able to work in those folders and push.
- Therefore, _you can skip the step of creating a new folder_ in chapters 2 and 3: you already have one.
- You will, however, need to add your own folders for part 4 and thereafter.

I'll float around and help.


## EXT: Tour of unit resources

If possible, I do want to give you a quick overview of the assets and advice I've compiled so far on [the course site's resources page]({{site.github.url}}/resources).

<div class="alert alert-info">
If you're already experienced at web design and/or you find yourself breezing through the Interneting is Hard tutorial, you can find other self-paced learning opportunities here.
</div>

<section id="vscode-extensions">
  <h3>Of particular note: Extensions for VS Code</h3>
   <p>NB: If there's something you expect VSCode to do, but it doesn't, chances are someone's already coded an Extension to make VSCode do it.</p>

  <div class="alert alert-info">
  To search for, install, or otherwise manage extensions, <strong>go to View > Extensions</strong> or click on the icon that looks like building blocks. You can search from the top bar.
  </div>

  <p>Some extensions I expect you'll find useful:</p>

  <ul>
        <li>
          <p><a href="https://marketplace.visualstudio.com/items?itemName=Compulim.compulim-vscode-closetag">Close HTML/XML tag</a>, by Compulim: adds a keyboard shortcut to automatically detect the last-opened html tag, and close it. Useful for proofreading!</p>
        </li>
        <li>
          <p><a href="https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag">Auto Rename Tag</a>, by Jun Han. If you change an <code class="language-plaintext highlighter-rouge">h2</code> to an <code class="language-plaintext highlighter-rouge">h3</code>, this will automatically update the corresponding closing or opening tag so you don’t end up with a mismatch.</p>
        </li>
        <li>
          <p><a href="https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek">CSS Peek</a>, by Pranay Prakash. Detects definitions for CSS <code class="language-plaintext highlighter-rouge">id</code>s and <code class="language-plaintext highlighter-rouge">class</code>es from inside your HTML files, by looking in linked stylesheets.</p>
        </li>
        <li>
          <p><a href="https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion">Intellisense for CSS Class Names in HTML</a>, by Zignd. Offers autocomplete for CSS <code class="language-plaintext highlighter-rouge">class</code> names from linked stylesheets while you’re working in HTML.</p>
        </li>
        <li>
          <p><a href="https://marketplace.visualstudio.com/items?itemName=george-alisson.html-preview-vscode">HTML Preview</a>, by George Oliveira (note that the more-frequently downloaded one, by Thomas Haakon Townsend, is no longer being maintained). Lets you see a preview of your HTML file without having to head to the browser (though you may still want to, for inspector reasons!)</p>
        </li>
        <li><a href="https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag">Auto-Close Tag</a>, by Jun Han. Every time you open a new HTML tag, the corresponding closing tag will be generated automatically. A lot of people love this, but I find it annoying; your mileage may vary.</li>
      </ul>

  <p>Read the README inside any installed package for tips on how to use it. This will open just like any other file, so you can move it, split it, etc.</p>
</section>


## Homework for Next Time

* **Do** as much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as time and interest allow – but *at least parts 1-4* (from "Introduction" through "Hello, CSS")
   - Heads up to fast workers: "float" layouts used to be a big deal, but aren't as widely recommended any more: modern techniques like grid and flex are more flexible, and easier to get right. You can probably skip that chapter, at least for now; the [Resources](../resources) page has links to some Grid tutorials.
* **Show your work** by pushing your tutorial code to GitHub, presumably inside your tutorials folder.
