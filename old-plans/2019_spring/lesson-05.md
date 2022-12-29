# Forward the Soundscape Foundation (Intro to Audacity)

1. Welcome back, and thanks for posting! (5 min)
2. Audacity Demo (10 min)
3. Audacity Play Time (20 min)
4. Command line redux: Versioning beyond GitHub (10 min)
5. Share and Enjoy (15 min)
6. HW Preview
7. EXT: Studio time and microconferences


## 1. Welcome back, and thanks for posting!

Many thanks to everyone for keeping the conversation going online, even when we weren't meeting face-to-face. I've read through all the posts as of 9pm last night, on both threads: the [blog post on listening to soundscapes](https://github.com/pitt-cdm/miller2019spring/issues/3) and your [soundscape narrative proposals](https://github.com/pitt-cdm/miller2019spring/issues/4).

Lots of overlap _and_ plenty of difference in the proposals, which is always a good thing. A bunch of you are working on days-in-the-life-of; you might find that you're able to divide and conquer some of the standard sounds, like pouring coffee or turning on a shower. Have a look through the queue and reach out to each other if you want to trade!

This is also, of course, a good reminder to try to find ways of making your story _your_ story, even as it takes on the conventions of a particular genre. If your proposal is focused on routine, what stories does your routine allow you to tell? If it's a game or a performance, what will draw listeners to this particular game or performance?

Remember, as well, that one tool you have in your toolkit is music, especially open-licensed music. **The [resources]({{site.github_url}}/resources) page of our website has lots of links and suggestions; please do make use of them!**

<!-- If by some miracle it's still 9:35, spend 5 minutes on Fair Use: purpose of copy, nature of original, substantiality of amount copied, market impact. -->

## 2. Audacity Demo (10 min)

I'm going to quickly walk through the basic features of Audacity, and then you're going to try your own hand at using them.

<div class="alert alert-info">
A more substantial introduction is available at the <a href="http://manual.audacityteam.org/man/audacity_tour_guide.html">Audacity Tour Guide</a>, so please review that if you find yourself stuck! (Google is also your friend, of course.)
</div>

### Import. Lay of the land.
Visual rendering of sound.

### Select tool; zoom tool.
Play a loop. Zoom. Selection adjust. Add label at selection.

### Time shift tool.
Split vs. split new. Mute/solo tracks.

### Save vs. export.
A project is an index to a folder full of sounds. You definitely want to save this! But to make it playable outside Audacity (and also a lot more transportable), export to mp3.

<div class="alert alert-danger">
To submit your full project in such a way that I can open it, you'll want to use the Git-LFS extension; more on that after playtime. For now, just know to always also export an mp3.
</div>

## 3. Audacity Play Time: Representative and Reprehensible Reporting

Your turn! Your mission is to produce two short clips (≤15 seconds) from the same 4ish-minute audio file, which I'm about to give you.

<div class="alert alert-info">
For clip 1, imagine something a reputable journalist might produce – a snippet meant to fairly represent a public figure's actual words and platform. In this clip, you should aim to condense without distorting, to make your 15-second highlight reel as true as possible to the spirit of the original.</div>

<div class="alert alert-info">
For clip 2, catching the listener's attention is all that matters. Here, anything is fair game in terms of editing: cutting out important words or sentences, rearranging things, stitching together unrelated pieces of speech. Your goal is to explore the transformative possibilities of digital audio editing – both for knowledge and defense – so see what kind of 15-second fake news you can produce from real materials.
</div>

We'll share these among each other, but not post to GitHub – we don't want any of our fake clips to circulate widely!

<div class="alert alert-success">
Today's audio clip is from <a href="{{site.github_url}}/uploads/pelosi-accepts-gavel-20190103.mp3">Nancy Pelosi's address to the House of Representatives on again being elected Speaker</a>, January 3, 2019. Download it, and get going!
</div>

<aside><smaller>
<strong>Credits</strong>

The audio was captured using Audacity and <a href="https://rogueamoeba.com/freebies/soundflower/">Soundflower</a> from <a href="http://houselive.gov/MediaPlayer.php?view_id=2&clip_id=12243">houselive.gov</a>, the website of the Office of the Clerk of the U.S. House of Representatives. The exercise is closely adapted from one by <a href="https://twitter.com/klynncameron/status/1039612472704069632">Kelsey Cameron</a>, who has been most kind in answering questions about audio pedagogy.
</smaller></aside>

<div class="alert alert-white">
<strong>EXT:</strong> If you've already finished both clips to your satisfaction, move on to extending git!
</div>

## 4. Command line redux: Versioning beyond GitHub (10 min)

Have a look at the project files you're saving. There's a single file with the .aup extension, and a folder ending in `_data` with dozens of little .au audio clips. Trust me when I say that **you do not want to upload this folder through the GitHub website**. It might not even work.

Last week, we ran out of time to talk about what we get by running git from the command line. Well, here are three things:

1. extended functionality
2. multi-file commits
3. time to problem-solve before sharing

I'll explain in more depth:

### Extended functionality

Git, like many other applications, supports plugins and add-ons. One that we need for this class is Git Large File Storage, or git-lfs. This extension allows us to store files "offsite" (i.e. not on GitHub) that would otherwise slow down our repositories to a crawl – while still having full access to those files locally *and* using our normal git workflow.

To install:

1. **If you're on a Mac with Homebrew,** type `brew install git-lfs` from any terminal window. (And if you're on a Mac without Homebrew, [get Homebrew](https://brew.sh/)! It makes life so much easier.)
2. **If you're on a PC with Git for Windows,** congratulations! It comes pre-installed with git-lfs.
3. **If you're on Chromebook**, try `crew install git-lfs`, but I don't know that it's been ported yet. :\ You can also try the direct download at [git-lfs.github.com/](https://git-lfs.github.com/).

To activate:

1. All systems: at a command line, type `git lfs install`

To set up to use with .au files:

1. In the folder with your soundscape repository, enter the following, one line at a time (i.e. press enter after each line):
```bash
git pull
git lfs track *.au
git add .gitattributes
git commit -m "track .au files with git lfs"
git push
```

<div class="alert alert-success">
If possible on your system, I want everyone to have done the Git LFS setup before you leave today!
</div>

### Multi-file commits
As you're saving your Audacity projects, your `_data` folder is going to be morphing and shifting, creating and deleting .au files all over the place.

When you're ready to record a commit message – that is, when you're ready to mark a save spot in your composing process, naming what actions you've just taken in your project – you can scoop up the entire folder in one go.

In the folder with your soundscape repository, enter the following, one line at a time:

```bash
git add *
git commit -m "your headline commit message" -m "your optional extra details"
```

Now everything in the folder is labeled with that single commit. (If you want to see what's happening, add in a `git status` around each of those lines.) Keep editing, and repeat the process at your next save spot!

<aside class="alert alert-info">
Note that the asterisk is a wildcard matching everything – or, rather, every file that's changed since it was last committed. If you prefer, you can `git add %filename%` for any filename one at a time, or use the asterisk to perform partial wildcard matching.
</aside>

### Time to problem-solve before Sharing

All those commits you just made are _local to your computer_: they're not shared yet. So you can try things out, make mistakes, and fix them before anyone stumbles onto your project and starts making judgments about quality.

When you're ready to push your projects to GitHub, type this in your command line (again, from the repository you want to share):
```bash
git push
```

Not only will that sync to GitHub, it'll also know which files you want to sync using Git Large File Storage, and make the transfer accordingly!


## 5. Share and Enjoy (15 min)
Before we have to go, let's hear at least a few of the 15-second clips you were able to produce from our Speaker of the House!


# Homework for next time:
<ul>
<li>If you didn't yet, please finish the work above!</li>
<li><strong>Work</strong> on your soundscape narratives, including making at least two recordings and putting them into conversation in Audacity. If you have time, do more!</li>
<li><strong>Push a soundscape preview</strong> to your GitHub repository, using the steps above. As per the assignment prompt, this should include:
  <ul>
  <li> A layered <strong>Audacity project file (.aup)</strong>, showing the arrangement of your sounds so far (need not be a complete soundscape or narrative yet).</li>
  <li> A static <strong><a href="https://www.take-a-screenshot.org/">screenshot</a></strong> (.png or .jpg) of your Audacity file in progress (for comparison later to subsequent drafts).</li>
  <li>The <strong>\_data folder</strong> associated with your Audacity file, which should contain at least two recorded sounds.</li>
  <li> A plain text (.txt) or markdown (.md) file, explaining in at least 300 words <strong>what you're showing us</strong> in this preview. Feel free also to ask questions or lay out next steps for yourself!</li>
  <li> An updated <strong>ASSETS.md</strong>, indicating which the files you've actually recorded or otherwise obtained. Add source documentation for any outside sources – and your permission to use them (e.g. licenses, fair use; see <em>Writer/Designer</em> p. 160-165).</li>
  </ul>
</li>
</ul>

## EXT: Studio time and microconferences

If we have time left, I'll be pleasantly surprised, but let's use it to get working on your proposed soundscape narratives!
