# GitHub and Git; Intro to Sound unit
**Texts to have read/watched:**

* Git and GitHub for Poets, starting at least with
[the Introduction](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)

**Work to have achieved:**

* Download and install what you need to use Git: at [the command line](https://gist.github.com/derhuerst/1b15ff4652a867391f03) and, optionally, using the [Desktop app](https://desktop.github.com)

## Plan for the day

1. GitHub Episode 2: Clone Warriors <!-- Ask: based on video, what's the diff btwn a clone and a fork?
Hmm. What should I have them clone? The Audacity assignment, but then we have to talk about it. Maybe the Five Affordances repo from last time. I can create a separate folder for images. -->
2. Multiple views of the same files: web, command line, Finder/Explorer
3. One more view: Atom interface <!-- Ben demo; what's made easy? -->
4. Now it's your turn! And also, here's the first project assignment<!-- Clone soundscape repo; open in Atom; rename README and make a new one -->
5. Audacity Tour, by way of a past-semester example (10-15 min) <!-- tracks, mute/solo, resize tracks, zoom, .aup files and the _data folder -->
6. Why we need Git Beyond GitHub
7. HW Preview



## 1. GitHub Episode 2: Clone Warriors

Last time, we saw how GitHub can let multiple people edit a file, integrate the changes, and keep track of the file's history. So far, so good!

But that was all text files. What happens when you want to work on something the web interface can't handle, like sound or images?

As it turns out, most of the time, you're going to want to have a *local copy* of your project that you can *pull* down from the clouds, make your changes on your own machine, and then *push* back up with the changes and history intact.

In git-speak, that linked local copy is called a *clone*. There are some good instructions (including pictures) in the GitHub documentation: [https://help.github.com/articles/cloning-a-repository](https://help.github.com/articles/cloning-a-repository).

Allow me to demonstrate by cloning the [Digital Affordances repo](https://github.com/benmiller314/cdm-digital-affordances) from last class.

## 2. Multiple views of the same files: web, command line, Finder/Explorer

When you clone a repository, it shows up on your computer as a folder, because *that's all a repository is: it's a file folder.* You can open it in Finder (Mac) or Explorer (Windows), and everything's arranged just the way you'd expect.

You can also open it via command line (a.k.a. _Terminal_ on Mac, or _GitBash_ or _PowerShell_ on Windows), and it's all just a different vantage point on the same location.

<details>
<summary>For more on the command line, click here to expand.</summary>
<h3>The command line: behind the scenes</h3>
<em>See also the <a href="https://youtu.be/oK8EvVeVltE">"Git and GitHub for Poets" episode 1.5, intro to the command line</a>.</em>

Much as a repository is just another name for a file folder you're tracking, the <em>command line</em> is just another way of seeing the files you're used to seeing in windows. (Note the lowercase 'w.') Instead of a graphical interface, everything here will be text.

If you're not sure how to open a command line, try <a href="https://learnpythonthehardway.org/book/appendix-a-cli/ex1.html">these instructions</a>.


<figure>
<img alt="terminal window showing git status command" src="../assets/img/terminal-git-status.png" />
<figcaption>Above, a terminal window. In the top line, the text to the left of the dollar sign ($) is a "prompt," showing where you are and who you're logged in as; text to the right are commands entered. Here, <code>git status</code> yields information about the repository's state (what's new, modified, or deleted since the last commit) and gives tips about how to proceed (last line before the return of the prompt).
</figcaption>
</figure>


<h3>To get where you're going:</h3>
<pre><code class="bash">
cd path/to/your/folder    # change directory
pwd               # print working directory (i.e. where am I?)
ls                # list directory contents
cd ..             # go up one directory level
cd ~              # go to home folder
open .            # open the current directory in Finder/Explorer
</code></pre>

NB: As a shortcut to the folder path in step one above, you can type <code>cd</code> (note the space) and just drag-and-drop the folder from Finder/Explorer into the command line.
NB: You can also press <code>tab</code> to autocomplete a partial file or folder name.

<div class="alert alert-info">
Change something in one view, and it changes in the other. Because it's really the same place.
</div>


<h3>Basic git workflow:</h3>
<pre><code class="bash">
git status           # see what git is tracking / what's changed
git pull             # download changes from GitHub
git status           # start of loop
# here you make changes to your files
git add %filename%   # optionally repeat
git status
git commit -m "your headline commit message - note the quotes" -m "your optional extra details, if you want them, just go in a second message."
                     # repeat add/commit loop as desired
git push             # publish your changes
</code></pre>

NB: Git may present you with some error messages, especially the first time you try to use it. Don't panic: <strong>read what the error message has to say!</strong> Most of the time, they'll give you some clear instructions on what to do to fix the problem.
</details>

<div class="alert alert-info">Note that GitHub Desktop is NOT showing you a view of your <em>files</em>, per se; it's showing you what's <em>changed</em> in your files.

But GH Desktop will helpfully offer to open the repository in Finder or Explorer... or in your preferred external text editor.
</div>

## 3. One more view: the Atom interface

### Initial questions to ask:

- How is the space of the app laid out?
- What's given the most prominent visual focus?
- What features/tools do you have quick access to?
  * for Atom: what do you get in the right-click menu?

I, for one, would like to reorganize these files. Here's how I would...

- create a subfolder
- move files into the folder

## 4. Now it's your turn! And also, here's the first project assignment

<div class="alert alert-success">
Head over to <strong><a href="https://github.com/benmiller314/soundscape2020fall">https://github.com/benmiller314/soundscape2020fall</a></strong>, then (1) <strong>fork</strong> the repo to take control of it, and (2) <strong>clone</strong> your fork to bring that new copy onto your hard drive.
</div>

Before we get too into the details, I want you to practice what I was just demoing:

(3) Open the repository in Atom.
(4) Change the name of the README.md file to **assignment.md**
(5) Create a new file in the repository, called README.md, and
(6) Fill it with some placeholder content, like, "This is the future site of Ben's soundscape narrative."

With that done, let's read through the assignment!
<!--
Go through overview, constraints, deadlines. Don't show parachute prompts except to say they exist.
-->

As I explained in the syllabus, your first project is to **arrange layers of sound to convey a sense of place and story.** In assigning this, I have two main goals for you:

1. to learn how to capture sound and edit it using digital tools, and
2. to explore the affordances of sound as a medium,

with particular attention to its ability to communicate
  - *immersive environment* and
  - *narrative pacing and change*.



## 5. Audacity Tour, by way of a past-semester example (10-15 min) <!-- tracks, mute/solo, resize tracks, zoom, .aup files and the _data folder -->

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

## 6. Why we need Git Beyond GitHub (10 min)

The number of files in the \_data folder can get quite large – easily into the hundreds. And the GitHub web interface, as great as it is, *cannot handle that many files at once*. Trying might well break your project.

So we'll need another solution.

Luckily, we have one! As you'll have learned from the videos, GitHub as a (mostly web-based) file-sharing and project-management platform is built on top of another system – Git – which runs mostly on text commands.

And Git can handle quite a bit more than GitHub can... and then share it seamlessly to GitHub, with all the hard work taken care of.

In particular:
<ul>
<li>Git lets you "stage" multiple files at once and wrap them in a single commit.</li>
<li>Git lets you keep track of changes locally (on your own computer) before you're ready to share them with the world – and then to "push" multiple commits all at once.</li>
<li>If you use the command line, you can also access and activate more features of Git than the GitHub defaults allow.</li>
</ul>

### Yet another view

Alternately, if you've downloaded [GitHub Desktop](https://desktop.github.com), you can use a visual interface to accomplish all of those local commands. And it'll also generously prompt you to push changes when you've finished committing them.

<!-- Ben quickly demos -->

<figure>
<img alt="github desktop shows status and diff view by default" src="../assets/img/github-desktop-status.png">
<figcaption>Above, Github Desktop. Checking the boxes at the left is akin to <code>git add</code>; uncheck to unstage individual files, as they'll all be selected by default. Commit messages are entered at the bottom left. A button to push is part of the toolbar at the top right.
</figcaption>
</figure>

(NB: If you haven't tried GH Desktop in a few years, it's vastly improved since around 2018.)



# HW for next time:
* **Download** the [Audacity](https://www.audacityteam.org/download/) audio editor, or update to the latest version if you already have it.
   - *Optionally* also download the [separate FFmpeg import/export library](https://manual.audacityteam.org/man/faq_installing_the_ffmpeg_import_export_library.html)<!-- NB: On Zoom, it might be helpful to have an additional audio input/output device like Soundflower or whatever the Windows equivalent is-->
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

* _Optional:_ This will be part of the homework next week, but if you want to get a head start, **read** the following advice on sound recording, **listening to the embedded clips**:
  - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).
  - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (**Note the time skips she recommends**: sometimes a long clip is embedded, but not meant to be listened to in full.)
