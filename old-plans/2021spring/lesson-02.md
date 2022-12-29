
# What Can We Do With Digital?

<!-- *** DON'T FORGET TO RENAME THE FILE, BEN! *** -->
<!--     Also: set up Zoom breakout groups  -->



**Texts to have read:**

* The [syllabus](/{{site.course.base_url}}uploads) and [grading contract](https://canvas.pitt.edu/courses/78948/modules)
* Su, ["Playing Lev Manovich"](https://tylersu.github.io/o/). Be ready to talk about what you noticed, and what you wondered.)

**Writing to turn in:**

* An open-book "quiz" on the grading contract
* A post to the main course [issue queue]({{site.github.issues_url}}/1), introducing yourself to your classmates (and anyone else who stumbles upon it)


## Plan for the Day

1. The Newness of New Media: Five Principles, in Brief (~15 min)
2. GitHub and Git <!-- repo, commit, history, diff --> (~15 min)
3. Five Principles as Lenses (~15 min)
4. Shareback (~15 min)
5. HW Preview

Welcome back! I really enjoyed reading all the introductory posts and letters; if you haven't had a chance to get to know your classmates' opening posts, I encourage you to [check them out]({{site.github.issues_url}}/1)!

### 1. Five Principles, in Brief

Can I get five people to fill us in on the five "principles of new media" from the webtext I asked you to read? i.e. One person, one term.

<!-- numerical representation, modularity, automation, variability,
and transcoding -->

Let's take notes here: [bit.ly/cdm2021spring-notes](http://bit.ly/cdm2021spring-notes)

<!-- Notice the Credits page: the ethics around using sources don't go away when you go digital. Copying is easy, and doesn't do direct harm to the original artifact... but it could cause reputational damage or lost opportunity to the original author.

Did anyone click through the links on the Credits? The original piece with the subtitle "Playing Lev Manovich" is now defunct, because it relied on Flash. That's another feature (or bug?) of digital media: ephemerality. One reason to prefer standards-based tools, rather than proprietary formats. Similarly, Su's original bio linked here is now gone: she stopped using the service. Another reason to learn how to roll your own. -->

### 2. GitHub, part 2
Last time, we saw that GitHub can host a discussion forum, so in that sense it's a community website: it makes media social.

But its core functionality is meant to solve a different media problem: tracking changes to files over time.

<figure role="figure">
  <a href="http://phdcomics.com/comics/archive.php?comicid=1531"><img src="../assets/img/cham-phd101212s.gif" style="height: 600px; height: 70vh; width: auto;" alt="webcomic shows a series of panels renaming final.doc to final_rev2, final_rev_6.comments, and so on to absurdity" title="I'm not the first to use this comic in a discussion of version control. See, for example, https://caltechlibrary.github.io/git-desktop/aio/."></a>
  <figcaption>from <a href="http://phdcomics.com/comics/archive.php?comicid=1531">PhD Comics</a> by Jorge Cham (2012).</figcaption>
</figure>

Renaming ever more files isn't only messy to keep track of: it also eats up your storage space, especially if you're working with multimedia. But digital media is all numeric, at heart, so we can instead just keep track of the *differences.*

<div class="alert alert-success">
Let's quickly walk through what it looks like to track changes via the GitHub.com web interface:
<strong><a href="https://github.com/benmiller314/text-demo#readme">https://github.com/benmiller314/text-demo</a></strong>
</div>

<!--
1. Create a new .txt file.
2. Demo the importance of the extension by previewing what happens if it's .md?
3. Commit the new file directly to master.
    - Note that the commit message has two parts: a short label, and a bigger box. These are kind of like the subject line of an email and the email body. The first is what you'll see automatically when browsing the history; the second will require an additional click. And GitHub will let you leave the "body" blank, but you're required to have a "subject line."
4. Change the text. *Ask for suggestions in the Zoom chat.*
5. Create a new branch, then merge it. Why, you ask?
   It matters when you're working with others: you want to make sure you're comparing against the most up-to-date version, so you don't accidentally erase something new.
   This will become important in a minute.
-->

### 3. Five Principles as Lenses

Time to take these abstractions and put them into practice, in two ways:

* practice using GitHub
* practice using our key terms to help us see differently

We'll be working in groups. I've used your Tech Comfort Survey responses from Lesson 1 to build breakout rooms where at least one person has prior GitHub experience, so I hope you'll be able to help each other where needed!

<div class="alert alert-success">
Head to
<strong><a href="https://github.com/benmiller314/cdm-digital-affordances#readme">https://github.com/benmiller314/cdm-digital-affordances</a></strong>, where you'll find more instructions for what to do next – starting with forking the repo. (Thanks, group GitHub anchors!)

Start by skimming through the instructions in the README file, so you know where this is headed. (It'll save you headaches later.)

Then follow the steps.
</div>

We'll work in Breakout Rooms for about 10-15 minutes, then report back. Don't forget that you can use Zoom chat and screenshare to your advantage.

Call me if you need me! Otherwise, I'll be floating from group to group.

## HW for next time:

* **Watch** Git and GitHub for Poets, starting at least with
[the Introduction](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV) and going as far as your interest and time allow.
  - I also especially recommend [1.5 / intro to the command line](https://youtu.be/oK8EvVeVltE) and [1.6 / clone, push, pull](https://youtu.be/yXT1ElMEkW8), though the latter gets a little long-winded... But then, that's what 1.5x playback is for, am I right?
* **Practice** following the steps in the video, using either a .txt file or a .md file: create a repository on GitHub, add some content to a file, commit, edit it, commit again, and view the history. Next class we can start with any questions that came up for you in the process.
   - If you've used GitHub a lot, you may want to play around with [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) formatting. Do you know what happens if you embed html inside a Markdown file? Or Markdown inside an html block?
* Download what you'll need to get git functioning **on your own computer** (i.e. not through the github.com website):
  - I highly recommend you download the **[GitHub Desktop application](https://desktop.github.com)**, available for MacOS or Windows, which (like the command line interface) has some essential features that are unavailable on the GitHub website.
  - *Alternatively:* you could install command-line git, probably using either GitBash (for Windows) or Homebrew (for Mac) – or see this [walkthrough of how to install git using, ironically enough, GitHub Desktop](https://www.techrepublic.com/article/how-to-install-github-desktop/#:~:text=That's%20right%2C%20even%20though%20GitHub,install%20Git%20(Figure%20B). (Linux users, I kind of assume you don't need further instructions, but hit me up if I'm wrong.)
  - *Extra optional:* Do you already know git basics, and want a more hands-on guide through the full GitHub functionality? See the GitHub Learning Lab entry on our [Resources page]({{site.github_url}}/resources).
