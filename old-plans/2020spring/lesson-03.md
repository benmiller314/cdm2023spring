



# GitHub and Git; Intro to Sound unit
**Texts to have read/watched:**

* Git and GitHub for Poets, starting at least with
[the Introduction](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)

**Work to have achieved:**

* Download and install what you need to use Git: at [the command line](https://gist.github.com/derhuerst/1b15ff4652a867391f03) and, optionally, using the [Desktop app](https://desktop.github.com)

## Plan for the day

1. GitHub for Poets review (15-25 min)
<!-- EXT. Versioning beyond simple text files -->
2. First project assignment: Soundscape Narrative (10-15 min)
3. Audacity Tour, by way of a past-semester example (10-15 min) <!-- tracks, mute/solo, resize tracks, zoom, .aup files and the _data folder -->
4. Git Beyond GitHub (10 min)
5. Multiple views of the same files
<!-- 6. A little command line setup for Soundscape Narrative -->
6. HW Preview


## 1. GitHub for Poets review (25 min)

<div class="alert alert-success">
<strong>Take 5 minutes or so to write on your own</strong>, from memory, about the video(s) you watched over the weekend: what stands out? what do you take away? what are you left wondering?
</div>

<div class="alert alert-info">

Next, <strong>in pairs, compare your impressions.</strong> Help each other with your questions; be ready to share remaining questions or big takeaways. Spend another 5-8 minutes here.
</div>

<em>EXT: What do you think are the limitations of the GitHub interface? What are some things you might want to do with Git that you haven't yet seen? Conversely, what do you think GitHub, as a website, might do better than Git at the command line?</em>

Okay, so **back to full-class discussion.** What are your takeaways? Your remaining questions?

## 2. First project: Soundscape Narrative (20 min)

As I explained in the syllabus, your first project is to **arrange layers of sound to convey a sense of place and story.** In assigning this, I have two main goals for you:

1. to learn how to capture sound and edit it using digital tools, and
2. to explore the affordances of sound as a medium,

with particular attention to its ability to communicate
  - *immersive environment* and
  - *narrative pacing and change*.

<div class="alert alert-success">
To read the full assignment – and fork a copy for yourself – go to <strong><a href="https://github.com/benmiller314/soundscape2020spring">https://github.com/benmiller314/soundscape2020spring</a></strong>.
</div>

Let's read through this together.

<!--
Go through overview, constraints, deadlines. Don't show parachute prompts except to say they exist. The sections below are prep for the "setup" section.
-->

## 3. Audacity Tour, by way of a past-semester example (10-15 min) <!-- tracks, mute/solo, resize tracks, zoom, .aup files and the _data folder -->

I want to start with a behind-the-scenes view of one of the finished soundscapes I'll ask you to listen to for homework.

This is Tyller Barner's "Coffeeshop Conversations," from Spring 2019. I'm very happy to talk at some point about the piece itself, but for now, let's see what it can show us about this new application, Audacity.

### Initial questions to ask:

- How is the space of the app laid out?
- What's given the most prominent visual focus?
- What features/tools do you have quick access to?

### Now let's play

<!--
1. Literally press play.
2. Zoom far in.
3. Pin the cursor.
4. Scroll up and down.
5. Zoom all the way out in one click.
6. View > Track Size > Collapse tracks.
7. Try to move "Hillman Coffee" track to the bottom. Can't do it without stopping!
8. Stop. Move the track. Hit play again. Where does it start?
9. Try muting the background noise.
10. Try muting the music track.
11. Rename the music track.
12. Revisit the questions above.
-->

### Project files vs. rendered files

<!-- show Tyller's files -->

<div class="alert alert-warning">
<strong>Important:</strong> Audacity project files, with extension .aup, do not in themselves contain any sound. They are, instead, an index of the files that live in an adjacent folder: if your main file is <em>project.aup</em>, then the data folder is <em>project_data</em>.

<strong>The .aup file and the \_data folder must always live in the same containing folder, and move together.</strong> If you have one in your repository but not the other, the project will not open properly!
</div>

NB: You should never need to manipulate the files in the \_data folder directly: just let Audacity handle them.

## 4a. Git Beyond GitHub (10 min)

The number of files in the \_data folder can get quite large – easily into the hundreds. And the GitHub web interface, as great as it is, *cannot handle that many files at once*. Trying might well break your project.

So we'll need another solution.

Luckily, we have one! As you'll have learned from the videos, GitHub as a (mostly web-based) file-sharing and project-management platform is built on top another system – Git – which runs mostly on text commands.

And Git can handle quite a bit more than GitHub can... and then share it seamlessly to GitHub, with all the hard work taken care of.

In particular:
<ul>
<li>Git lets you "stage" multiple files at once and wrap them in a single commit.</li>
<li>Git lets you keep track of changes locally (on your own computer) before you're ready to share them with the world – and then to "push" multiple commits all at once.</li>
<li>If you use the command line, you can also access and activate more features of Git than the GitHub defaults allow.</li>
</ul>


### Clone Warriors
All of that depends on getting your files from GitHub onto your own computer, while still keeping them linked and tracked.

Which means it's now time to **[*clone* the repository you just created](https://help.github.com/articles/cloning-a-repository/)**: that is, let's download it and make sure we're still tracking it with the same Git commit history.

<figure>
<img alt="github clone or download button" src="../assets/img/github-clone-or-download.png" title="The clone button is just above the list of files, on the right." />
</figure>

There are three ways...

<figure>
<img alt="github clone or download button, open" src="../assets/img/github-clone-or-download-2.png" />

<figcaption>
<ul><li> <!-- The most obvious is --> download zip (but I don't recommend this)</li>
<li>command line: <code>git clone %clone_url%</code></li>
<li>open in desktop (I recommend this)<ul><li>If you haven't yet downloaded GH Desktop, it'll automatically redirect you to a page where you can.</li></ul></li></ul>
</figcaption>

</figure>

<figure>
<img alt="github open in desktop – choose file location" src="../assets/img/github-clone-where-to-save.png" />
<figcaption>Click that little "choose" button to get a dialog box, letting you put the files somewhere you can access them easily. <!-- And don't panic if you get an error that the location already contains files! Just click the "choose" button and go somewhere else. --></figcaption>
</figure>


## 5. Multiple Views of the Same Files

Where do the files go when you clone them? You could use Windows Explorer or Mac Finder to open the folder you just saved to...

... but how to do commits there? How to see file history?


### The command line: behind the scenes
_See also the ["Git and GitHub for Poets" episode 1.5, intro to the command line](https://youtu.be/oK8EvVeVltE)._

Much as a repository is just another name for a file folder you're tracking, the <em>command line</em> is just another way of seeing the files you're used to seeing in windows. (Note the lowercase 'w.') Instead of a graphical interface, everything here will be text.


The command line goes by many names: a.k.a. _Terminal_ on Mac, or _GitBash_ (or _PowerShell_) on Windows. If you're not sure how to open it, try <a href="https://learnpythonthehardway.org/book/appendix-a-cli/ex1.html">these instructions</a>.


<figure>
<img alt="terminal window showing git status command" src="../assets/img/terminal-git-status.png" />
<figcaption>Above, a terminal window. In the top line, the text to the left of the dollar sign ($) is a "prompt," showing where you are and who you're logged in as; text to the right are commands entered. Here, <code>git status</code> yields information about the repository's state (what's new, modified, or deleted since the last commit) and gives tips about how to proceed (last line before the return of the prompt).
</figcaption>
</figure>


**To get where you're going:**
```bash
cd path/to/your/folder    # change directory
pwd               # print working directory (i.e. where am I?)
ls                # list directory contents
cd ..             # go up one directory level
cd ~              # go to home folder
open .            # open the current directory in Finder/Explorer
```

NB: As a shortcut to the folder path in step one above, you can type `cd ` (note the space) and just drag-and-drop the folder from Finder/Explorer into the command line.
NB: You can also press `tab` to autocomplete a partial file or folder name.

<div class="alert alert-info">
Change something in one view, and it changes in the other. Because it's really the same place.
</div>


**Basic git workflow:**
```bash
git status           # see what git is tracking / what's changed
git pull             # download changes from GitHub
git status           # start of loop
# here you make changes to your files
git add %filename%   # optionally repeat
git status
git commit -m "your headline commit message - note the quotes" -m "your optional extra details, if you want them, just go in a second message."
                     # repeat add/commit loop as desired
git push             # publish your changes
```

NB: Git may present you with some error messages, especially the first time you try to use it. Don't panic: **read what the error message has to say!** Most of the time, they'll give you some clear instructions on what to do to fix the problem.

<!-- Ben quickly demos -->

### Yet another view

Alternately, if you've downloaded [GitHub Desktop](https://desktop.github.com), you can use a visual interface to accomplish all of those local commands. And it'll also generously prompt you to push changes when you've finished committing them.

<!-- Ben quickly demos -->

<figure>
<img alt="github desktop shows status and diff view by default" src="../assets/img/github-desktop-status.png">
<figcaption>Above, Github Desktop. Checking the boxes at the left is akin to <code>git add</code>; uncheck to unstage individual files, as they'll all be selected by default. Commit messages are entered at the bottom left. A button to push is part of the toolbar at the top right.
</figcaption>
</figure>

(NB: If you haven't tried GH Desktop in a few years, it's vastly improved since then.)

## 4b. Back to Git Beyond GitHub

<div class="alert alert-success">
With all that settled, let's finally take advantage of Git outside of GitHub, and <strong>make two changes in the same commit:</strong>

<ol>
<li>rename the README.md file to ASSIGNMENT.md, and</li>
<li>create a new README.md file that describes, in your own words, what you think you might make in this space. (Don't worry, you can always change it later.)</li>
</ol>
Then <em>push</em> your changes so they appear on GitHub.
</div>

Atom editor would be especially useful here!

EXT: If you're already good with all this – e.g. if you've used Git before – please help others who are catching up.




# HW for next time:
* **Download** the [Audacity](https://www.audacityteam.org/download/) audio editor, or update to the latest version if you already have it.
   - *Optionally* also download the [separate FFmpeg import/export library](https://manual.audacityteam.org/man/faq_installing_the_ffmpeg_import_export_library.html)
* **Bring** headphones – we should have time to practice using it!

* **Listen** to the following recordings made by students in response to a similar prompt:
<!-- update each time with examples from this class where possible -->
  - Barner, Tyller. "Coffee Shop Conversations." *Digital Media and Pedagogy Showcase Spring 2019.* [http://dmap.pitt.edu/node/248](http://dmap.pitt.edu/node/248).
  - Funke, Taylor. "Soundscape - Day In: Day Out." *Digital Media and Pedagogy Showcase Spring 2018.* [http://dmap.pitt.edu/node/177](http://dmap.pitt.edu/node/177).
  - Quaid, Fatema. "A Haunted Halt." *Digital Media and Pedagogy Showcase Fall 2019.* [http://dmap.pitt.edu/node/295](http://dmap.pitt.edu/node/295).
  - Wick, Thomas. "Soundscape - Expedition to Planets Unknown." *Digital Media and Pedagogy Showcase Spring 2018.* [http://dmap.pitt.edu/node/178](http://dmap.pitt.edu/node/178). (NB: starts loud; turn volume down)

* **Listen**, as well, to the following audio tracks from the first few minutes of successful TV dramas:
  - [Breaking Bad]({{site.github_url}}/assets/sound/bb-pilot-opening.mp3). Sound extracted from https://www.youtube.com/watch?v=D-G8weg2Ndg under Fair Use, for instructional purposes.
  - [Battlestar Galactica]({{site.github_url}}/assets/sound/bg-pilot-opening.mp3). Sound extracted from https://www.youtube.com/watch?v=9VBTcDF1eVQ under Fair Use, for instructional purposes. (NB: starts very quiet)

* **Write** a short blog post to the appropriate thread [on the issue queue]({{site.github.issues_url}}): What do you notice, i.e. what stands out while reading or listening? What does that suggest, or what does it make you wonder?

<hr/>

* _Optional:_ This will be part of the homework for the weekend, but if you want to get a head start, **read** the following advice on sound recording, **listening to the embedded clips**:
  - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).
  - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (**Note the time skips she recommends**: sometimes a long clip is embedded, but not meant to be listened to in full.)
