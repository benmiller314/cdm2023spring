
# Digital Affordances


**Texts to have "read":**

* Tyler Su's ["Playing Lev Manovich"](https://tylersu.github.io/o/)
* Sample sound narratives

**Writing to turn in:**

* A post to the main course [issue queue]({{site.github.issues_url}}/2), reflecting on what you noticed and wondered in your reading/playing/listening

## Plan for the day

<!--

I. Five Principles of New Media
  1. What does this help you see about "digital" that wasn't part of the story you told last time?

II. Continuing where we left off: Clone, Edit, Push, Pull
  1. Re-open and *clone* the cdm-gh-practice repository you used last time.
  2. Ask the standard questions of GH Desktop: what's made easy in this interface? What kinds of things are in the menu? Context menu?
  3. Open the repo in Atom (or your preferred text editor). If you don't see it, set your editor in preferences.
  4. Explore the Atom interface: file navigation on the left, files in the main space. Ask the standard questions: what's made easy in this interface?
  5. Change something in your story.
  6. Go back to GH Desktop. Commit the changes.
  7. Push to origin (it really wants you to!)
  8. Pull the changes from your groupmates.
  EXT: merge errors; reverting

III. The audio project, assigned.
  1. Read it Together
  2. Clone it
  3. Open in Atom and rename the README to assignment.md
  4. Create a new file called README and put in some filler text.
  5. Push changes.

IV. Assign homework (i.e. save the Audacity Tour for lesson-04)

 -->

1. What's different about digital again?
2. Continuing where we left off: clone and edit, push and pull
3. Audio unit assignment
4. Homework preview


## 1. What's different about digital, again?

Can I get five people to recap the five "principles of new media" from the webtext I asked you to read? i.e. One person, one term.

<!-- numerical representation, modularity, automation, variability,
and transcoding -->

**Let's take notes here:** [bit.ly/cdm{{site.course.slugterm}}-notes](http://bit.ly/cdm{{site.course.slugterm}}-notes). Any volunteers to be in charge of notes for today? Usually 2-3 people works best...

<!-- Notice the Credits page: the ethics around using sources don't go away when you go digital. Copying is easy, and doesn't do direct harm to the original artifact... but it could cause reputational damage or lost opportunity to the original author.

Did anyone click through the links on the Credits? The original piece with the subtitle "Playing Lev Manovich" is now defunct, because it relied on Flash. That's another feature (or bug?) of digital media: ephemerality. One reason to prefer standards-based tools, rather than proprietary formats. Similarly, Su's original bio linked here is now gone: she stopped using the service. Another reason to learn how to roll your own. -->

What do these framing concepts help you see about "digital" that wasn't part of the story you told in your group last class?

I had you pair this reading with listening to several audio narratives. What does putting these things together help you notice or better understand – about either the audio narratives or about the concepts?


## 2. Return of the GitHub: clone and edit, push and pull

Last time, we saw how GitHub can let multiple people edit a file, integrate the changes, and keep track of the file's history using the GH website. But what if you want to change multiple files at once? What if you want to track history for files that aren't text, and can't be edited directly on their website?

As it turns out, most of the time, you're going to want to have a *local copy* of your project that you can *pull* down from the clouds, make your changes on your own machine, and then *push* back up with the changes and history intact.

In git-speak, that linked local copy is called a *clone*. There are some good instructions (including pictures) in the GitHub documentation: [https://help.github.com/articles/cloning-a-repository](https://help.github.com/articles/cloning-a-repository).


### 2a. Clone
Let's **practice by cloning the [CDM GH Practice repo](https://github.com/benmiller314/cdm-gh-practice) from last class – your own fork of that project**, so you're able to submit changes to it. (If you've lost your fork, you can find it again by clicking on either your profile or on the number of forks in the description block. The latter will show you all the forks of the project you're viewing, and the former will show you all the repositories you're a member of.)

<figure>
<img src="{{site.github_url}}/assets/img/github--clone-and-find-forks.png" alt="screenshot of github website description block, highlighting Code button (to clone), Forks, and Profile" />
</figure>

When given the option, choose "Open in GitHub Desktop."

### 2b. The GitHub Desktop interface

I zoomed through this too quickly last time:

1. How is the space laid out?
  * What can you see? What can't you see that you expected to, if anything?
2. What's given the most prominent visual focus? Secondary focus?
3. What features/tools do you have quick access to?
  * For instance, what's featured in the menu? What about the context menus (e.g. when you right-click)?
  * Do any of those tools let you find what you were missing?


### 2c. The Atom Interface

Let's take advantage of one of those featured options to open the repository in your preferred text editor.

And then let's ask those same questions again:

1. How is the space laid out?
  * What can you see? What can't you see that you expected to, if anything?
2. What's given the most prominent visual focus? Secondary focus?
3. What features/tools do you have quick access to?
  * For instance, what's featured in the menu? What about the context menus (e.g. when you right-click)?
  * Do any of those tools let you find what you were missing?


Let's practice:
* adding a new file
* changing a filename
* splitting the screen to show two files at once

Go ahead and **make a change to your story from last time, and save it.** (Not sure what to add? Maybe incorporate an example of modularity, automation, variability, or transcoding.)

Where does the change happen? Who can see your changes?

### 2d. Back in GH Desktop...

**Write a commit message** in the bottom left. (Make sure it's meaningful.) Before you click "commit," make sure you've selected the files you want to include under this version.

### GH Desktop FAQ
<details><summary>What if I realize I made a mistake in my last commit?</summary>

Go to the History tab, and right-click the last change (which will be on the top). You have options!

</details>
<details><summary>What if I already pushed my mistake to the cloud?</summary>

That's trickier. Here, to undo, you're probably going to need to add. While there are ways to "alter history," they're a little riskier than just reverting. Instead, you'll need to "revert" the change, which results in a new commit. (In GH Desktop, you can again find this in the right-click menu of the History tab.)
</details>

<details><summary>If I revert an old save, why don't I go back to that point in time?</summary>

Remember that each commit is a record of the **difference** between two states. So by reverting that difference, you're undoing that particular change. (This can be beneficial!)

</details>
<details><summary>So what do I do if I actually want to roll back all the way to a particular old commit?</summary>

The easiest option is to right-click that point in the History, then choose "create branch from this commit." You'll find yourself in a workspace identical to that point in time... but without destroying the work you've done since.

</details>
<details><summary>I tried that branch thing. You said it wouldn't destroy anything, so where are all my files?!?</summary>

When you "check out" a branch, the only files you can see are the ones on that branch. The others get hidden away inside the .git folder (which I strongly urge you not to open). If you were to switch back to the branch from before, you'd be back in that timeline, and the files would change accordingly. To merge branches back together, you just need to file a pull request and actively commit to the merge. In GH Desktop, you'll find both options (switch and pull request) under the "Branch" menu.

</details>

## 3. Another repo to fork and clone: the Audio Narrative assignment

<div class="alert alert-success">
Head over to <strong><a href="https://github.com/benmiller314/soundscape2022spring">https://github.com/benmiller314/soundscape2022spring</a></strong>, then (1) <strong>fork</strong> the repo to take control of it, and (2) <strong>clone</strong> your fork to bring that new copy onto your hard drive.
</div>

### 3a. First, let's read!

As I explained in the syllabus, your first project is to **arrange layers of sound to convey a sense of place and story.** In assigning this, I have two main goals for you:

* to learn how to capture sound and edit it using digital tools, and
* to explore the affordances of sound as a medium, with particular attention to its ability to communicate
  - *immersive environment* and
  - *narrative pacing and change*.

The README file has additional constraints, which I hope are generative; deadlines to give a rhythm to your production, review, and revision; and some "parachute prompts" if you feel lacking in direction and a deadline's coming up.

<!--
Go through overview, constraints, deadlines. Explain about parachute prompts.
-->

### 3b. Then, let's practice that edit / commit / push cycle!

(3) Open the repository in Atom.
(4) Change the name of the README.md file to **assignment.md**
(5) Create a new file in the repository, called README.md, and
(6) Fill it with some placeholder content, like, "This is the future site of So-and-So's audio narrative." You can (and should!) update this later.

Save your changes, and we can head back to GitHub Desktop. Note that, unlike github.com, GH Desktop...
<ul>
<li>lets you "stage" multiple files at once and wrap them in a single commit.</li>
<li>lets you keep track of changes locally (on your own computer) before you're ready to share them with the world – and then to "push" multiple commits all at once.</li>
<li>makes it easier to undo or amend the most recent commit</li>
</ul>

NB: If you use the command line, you can also access and activate even more features of Git than graphical interfaces allow. I'm going to drop this here, in case anyone finds they need it: [https://ohshitgit.com/](https://ohshitgit.com/) (or the more kid-friendly [https://dangitgit.com/](https://dangitgit.com/)).


<div class="alert alert-success">
<p>If you haven't yet done so, please...
(7) Commit the changes you made above: a new name for the old README.md file, and a new README.md with your own content. Then go ahead and (8) push back to GitHub.</p>

<p>NB: This is how I'll expect you to turn in all major assignments and meet interim deadlines toward them. It's also how I'll confirm  attendance for asynchronous participation in today's class.</p>
</div>


## HW for next time:
* **Download** the [Audacity 3](https://www.audacityteam.org/download/) audio editor, or update to the latest version if you already have it.
   - NB: some source sites will try to trick you into downloading unrelated software. Don't fall for it. Start on the audacityteam.org, and read the links carefully.
   - *Optionally* also download the [separate FFmpeg import/export library](https://manual.audacityteam.org/man/faq_installing_the_ffmpeg_import_export_library.html), which expands the file types Audacity can handle. Might be useful for imports from your phone, depending on your device!
   - *Optionally* download a phone recording app. Your device may already have a decent default voice recorder that you can use; let the class know if you have suggestions (or anti-suggestions).
<!-- * **Bring** headphones – we should have time to practice using it! -->
* **Watch** this recommended [Audacity 3 tutorial](https://www.youtube.com/watch?v=8oOaXWdmMcc) (about 20 minutes long) and come in ready to play with the software (and ask any questions that come up)


<hr/>

_Optional:_ This will be part of the homework for next week, but there's a bunch of stuff over the weekend. If you want to get a head start:

- The term "asset" comes from the book _Writer/Designer_ (Ball, Sheppard, and Arola, eds). A scan of the relevant chapter is <a title="not posted to preserve the limited distribution that helps justify my fair use claim (as does my colorless copy and the limited amount copied, relative to the book)" href="{{site.canvas_url}}/assignments/849366">posted to the Perusall social annotation software on Canvas</a>; I'll ask you to read it before writing your proposal.

- I'll also ask you to read the following advice on sound recording, _listening to the embedded clips_:
  - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).

  - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (**Note the time skips she recommends**: sometimes a long clip is embedded, but not meant to be listened to in full.)
