# GitHub and Git; Intro to Sound unit
**Texts to have read/watched:**

* Git and GitHub for Poets, starting at least with
[the Introduction](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)

**Work to have achieved:**

* Download and install what you need [to use Git at the command line](https://gist.github.com/derhuerst/1b15ff4652a867391f03)

## Plan for the day

1. GitHub for Poets review (25 min)
<!-- EXT. Versioning beyond simple text files -->
2. First project: Soundscape Narrative (20 min)
3. What Git does better than GitHub (5 min)
4. Very Brief Intro to the Command Line: going behind the scenes (but the usual scenes)
5. A little command line setup for Soundscape Narrative
6. HW Preview


# 1. GitHub for Poets review (25 min)

<div class="alert alert-success">
<strong>Take 5 minutes or so to write on your own</strong>, from memory, about the videos you watched over the weekend: what stands out? what do you take away? what are you left wondering?
</div>

<div class="alert alert-success">

<strong>In pairs, compare your impressions.</strong> Help each other with your questions; be ready to share remaining questions or big takeaways. Spend another 5-8 minutes here.

<em>EXT: How well do you think GitHub can track Word files? Try it on one of your own repositories and see what happens if you upload two different versions of the same file.</em>

</div>

Okay, so **back to full-class discussion.** What stands out?

# 2. First project: Soundscape Narrative (20 min)

As I explained in the syllabus, your first project is to **arrange layers of sound to convey a sense of place and story.** In assigning this, I have two main goals for you:

1. to learn how to capture sound and edit it using digital tools, and
2. to explore the affordances of sound as a medium,

with particular attention to its ability to communicate
  - *immersive environment* and
  - *narrative pacing and change*.

<div class="alert alert-success">
To read the full assignment – and make a copy for yourself – go to <strong><a href="https://classroom.github.com/a/9O5NEFUj">https://classroom.github.com/a/9O5NEFUj</a></strong>.
</div>

Let's read through this together.

<!--
Go through overview, constraints, deadlines. The sections below are prep for the "setup" section.
-->

# 3. What Git does better than GitHub

As you'll have learned from the videos, GitHub is a (mostly web-based) file-sharing and project-management platform built on top of Git – the version control system that runs mostly on text commands. GitHub's pretty, well, pretty.

<div class="alert alert-info">
Let's pause for a moment: <strong>Why would we ever want to use Git outside of GitHub?</strong>
</div>

<!--
Super-technical people may have many more reasons than I want to get into. For today, let's focus on a few quick victories:

* Git lets us "stage" multiple files at once and wrap them in a single commit.
* Git lets us keep track of small changes locally before we're ready to share them with the world – and then to push multiple commits all at once.
* Using the command line lets us access and activate more features of Git than the GitHub defaults allow.

We're going to practice this now.
-->

Okay, with that settled, it's time to [*clone* the repository you just created](https://help.github.com/articles/cloning-a-repository/): that is, let's download it and make sure we're still tracking it with the same Git commit history.

Then, let's make two changes in the same commit: rename the README.md file to ASSIGNMENT.md, and create a new README.md file that describes, in your own words, what you think you might make in this space. (Don't worry, you can always change it later.)


# 4. Very Brief Intro to the Command Line: going behind the scenes (but the usual scenes)

Much as a repository is just another name for a file folder you're tracking, the command line is just another way of seeing the files you're used to seeing in windows. (Lowercase 'w.')

<div class="alert alert-warning">
Not sure how to open a command line? Try <a href="https://learnpythonthehardway.org/book/appendix-a-cli/ex1.html">these instructions</a>.
</div>

To get where you're going:
```bash
cd path/to/your/folder    # change directory
ls                # list directory contents
```

Download the folder, preserving the connected history:
```bash
git clone %clone_url%
```
<div class="alert alert-warning">
NB: Don't include those percent signs; that's just my way of saying that <em>clone_url</em> is a variable, not a literal string you need to type in.
</div>

Core commands you'll need often:

```bash
git status           
git pull             # download changes from GitHub
git status           # start of loop
git add %filename%    
git status
git commit -m "your headline commit message" -m "your optional extra details, if you want them, just go in a second message."
                     # repeat loop as desired
git push             # publish your changes
```

<div class="alert alert-info">
<strong>NB:</strong> Edits that you make outside of the command line are reflected in the command line. Why? Because <em>it's the same folder, just viewed from a different vantage point.</em>
</div>

## 5. A little command line setup for the Soundscape Narrative

Armed with that primer, let's do one more thing at the command line before you go out and start recording and editing soundscapes.

<div class="alert alert-success">
<a href="https://github.com/pitt-cdm/soundscape-prompt#setup" class="alert-link">Head back into the assignment prompt, and scroll down to Setup.</a>
</div>

# HW for next time:
<!-- move this first part to follow lesson 4? -->
* **Read** the following advice on sound recording, **listening to the embedded clips**:
  - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).
  - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (Note the time skips she recommends: sometimes a long clip is embedded, but not meant to be listened to in full.)

* **Listen** to the following recordings made by students in response to a similar prompt:
<!-- update next time with examples from this class where possible -->
  - Cestare, Jessica. "Soundscape - The Dark Side of The Cat in the Hat." *Digital Media and Pedagogy Showcase Spring 2018.* [http://dmap.pitt.edu/node/176](http://dmap.pitt.edu/node/176). Accessed 15 Jan. 2019.
  - Funke, Taylor. "Soundscape - Day In: Day Out." *Digital Media and Pedagogy.* [http://dmap.pitt.edu/node/177](http://dmap.pitt.edu/node/177). Accessed 15 Jan. 2019.
  - Wick, Thomas. "Soundscape - Expedition to Planets Unknown." *Digital Media and Pedagogy Showcase Spring 2018.* [http://dmap.pitt.edu/node/178](http://dmap.pitt.edu/node/178). Accessed 15 Jan. 2019.
  - White, Zach. "Soundscape - Expanded Space." *Digital Media and Pedagogy Showcase Spring 2018.* [http://dmap.pitt.edu/node/195](http://dmap.pitt.edu/node/195). Accessed 15 Jan. 2019.

* **Listen**, as well, to the following audio tracks from the first few minutes of successful TV dramas:
  - [Breaking Bad]({{site.github_url}}/assets/sound/bb-pilot-opening.mp3). Sound extracted from https://www.youtube.com/watch?v=D-G8weg2Ndg under Fair Use, for instructional purposes.
  - [Battlestar Galactica]({{site.github_url}}/assets/sound/bg-pilot-opening.mp3). Sound extracted from https://www.youtube.com/watch?v=9VBTcDF1eVQ under Fair Use, for instructional purposes.

* **Write** a short blog post [on the issue queue](https://github.com/pitt-cdm/miller2019spring/issues/3): What do you notice, i.e. what stands out while reading or listening? What does that suggest, or what does it make you wonder?
