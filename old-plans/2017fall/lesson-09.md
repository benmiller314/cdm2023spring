## Layering Sound

**Texts to have read**: 

* Two versions of John Bresland's "Future Ex Buys Pajamas," first as <a href="http://brevitymag.com/nonfiction/future-ex-buys-pajamas/">written</a> and then as <a href="http://bresland.com/audio.html">recorded</a>
* Ira Glass on <a href="https://www.youtube.com/watch?time_continue=322&v=5pFI9UuC_fc">storytelling for broadcast</a>

**Work to have done**:

* A brief reflection on the WordPress site: what do you notice in putting these texts together? what does that make you wonder? 
* Brainstorming about what piece you'll remediate, with a couple of options to talk through with your groupmates


<!--
[toc tag="h2" title="Plan for the Day"]
-->


### Git and GitHub, Revisited

I'm going to walk us through some setup. If you're already a pro at this, including git-lfs, you can use the time to work on your audio project.

* Keeping things in sync
 - DO NOT separately create a local folder and a repository online: it leads to badness.
 - if you start online, **clone that** to your desktop
 - if you start locally, **publish that** to GitHub
 
Before we move on, let's all do that.
 
#### The command line: going backstage
* Mac users, run *Terminal*; Windows users, run *cmd*.
* `cd` = change directory. 
 - you can drag a file or folder from your GUI into the command line, and it'll paste the "path" to the directory for use with `cd`.
* `ls` = list directory contents. Often the first thing you do when you get to a new directory. Some variants I often find useful:
 - `ls -a`: list *all* directory contents. Shows hidden files! Important.
 - `ls */`: show subdirectories and their contents. Useful for navigating.

#### Using Git LFS for Large File Storage 
* Follow steps at [https://git-lfs.github.com/](https://git-lfs.github.com) ![download, initialize, instruct, and carry on]({{site.baseurl}}/assets/img/screenshot_installing-git-lfs.png)
 - Optionally, install homebrew: [https://brew.sh/](https://brew.sh). This is a command line "package manager" for Mac; essentially, it makes it significantly easier to install open source apps that you won't find in the AppleStore.
 - NB: if you don't have git itself installed, this won't work! Grab yourself a copy from [https://git-scm.com/downloads](https://git-scm.com/downloads)... or install via Homebrew with `brew install git`. More details in the [Git official documentation](https://git-scm.com/book/en/v1/Getting-Started-Installing-Git).
* In the first part of step 2, you'll at least want to repeat that step with *.aup, *.au, *.mp3, and probably *.xcf and *.tgz as well.
* Finally, in the second part of step 2, you'll need to add, commit, and push your `.gitattributes` file (glad we can now find hidden files!)

Thankfully, once you set this up via the command line, it should work pretty seamlessly with the GitHub desktop app!

NB: If you get prompted to log in over and over, try going back to the command line and, in the directory you're tracking, type this (thanks, [issue queue](https://github.com/git-lfs/git-lfs/issues/203)!):
```
git config --global credential.helper cache
```
<!-- The error is apparently caused by LFS using http instead of https, prompting your system to doubt your authenticity, per [this tutorial](https://github.com/git-lfs/git-lfs/wiki/Tutorial). --> That should turn on a setting that stores your current username and password, and tries that first before prompting you again.


### Whew! Can we get back to audio now?

#### Sound as extra layer
As a reward for getting through that, here's some Star Wars:
https://www.youtube.com/watch?v=zqZ0WRZmDfQ&feature=youtu.be&t=1m31s

And here's that same clip, modified:
https://www.instagram.com/p/BEZj3YMyAk_/?taken-by=starwars.remastered

Thoughts?

#### Reflections from the homework (save 20-30 min for groups!)
Let's link this to Bresland now, and what changed for you when you heard the audio. NB: Let's try to limit this to 

Most of you commented on the surprise of the tone; some liked it (several used words like "seductive" or "sultry"), some didn't, but all agreed that it changed things:

> Bresland's tone was sort of eerie; it made the essay so suspenseful compared to the original. (Alyssa)
 
> His breathy tone is really alienating, like he's right next to you.  It doesn't make me interested, doesn't draw my attention to content, it makes me want to turn it off.  I tried to listen to this all the way through twice and failed twice.
> 
> I realize that Bresland likely intended to make us slightly uncomfortable, but I doubt he wanted us to run away from him like I wanted to. (Gabi)

> the sequence in which I experienced these versions is important is because the text reading me was more open minded and willing to consider multiple reasons for Bresland's tone.  I don't think I would have been able to overcome my feelings about the audio versions before reading the text, and my observations would have remained firm and been consistent when my eyes hit the page. (Gwen)

Several of you paid attention to pauses, by both Bresland and Glass:

>  I also notice specific details more. The specific imagery, like chickens, burning leaves, erotic glances, and black stockings, are emphasized by the silences the speaker leaves and the accent sounds that either overlapped or followed the words. Near the end when he says the paragraphs about being a victim of his own manhood, the lack of background sound makes the paragraph seem incredibly long even though it is just a small portion of the work. (Casey T)

> Ira Glass [...] goes through step by step of storytelling by also building a kind of suspense. He pauses and emphasizes certain words. His tone also shows that he is fully invested into what he is saying, which makes me want to pay attention more. (Casey R)

And, just to follow up on that last comment, here's one more linking the two pieces based on storytelling and attention:

> Another building block he [Glass] mentioned was to raise questions throughout the story, which I noticed in the text we read from the last line of the first paragraph when Bresland said, “She says no Parisian would be caught dead anywhere near the Eiffel Tower, and by the end of the first day I know that she’s right.” We don’t know what’s going to happen throughout the rest of the day, but this foreshadowing tells us that we will soon have some sort of answer to why this is the case, as we continue reading. (Jappmann)


Anything else we're missing in this discussion?


### Group brainstorming

<div class="alert alert-success">
Use the remaining class time (less five minutes to introduce the homework) to share your ideas with your groupmates. <strong>What text might you want to re-cast as audio? What kinds of sounds or music might you layer in, for what kind of tone?</strong>

Take turns, and use <em>active listening</em> – that is, say back the heart of what you hear, with a <strong>...?</strong> at the end – to open a space for your partners to clarify and expand.
</div>

Before you leave and get distracted, jot down some notes.


## For Next Time
* **Inputs**
 * **Read and listen to** Bresland's <a href="http://bresland.com/brevity.html">"On Writing for the Ear"</a>, in which he narrates and explains the choices he made that led him to the recording you heard for today.
 * **Read and listen to** Rob Rosenthal's HowSound on <a href="https://transom.org/2017/sound-design-basics/">Sound Design Basics</a>
  * EXT inputs for eager audiophiles: HowSound on <a href="https://transom.org/2017/avoiding-pesky-recording-problems/">Avoiding Pesky Recording Problems</a> and <a href="http://training.npr.org/audio/the-ear-training-guide-for-audio-producers/">NPR's ear training guide for advanced audio editing</a>.
  * NB: I'm not expecting you to buy expensive equipment! If you want to up your recording quality beyond your laptop or phone microphone, you can borrow some from the Media Lab: http://dmap.pitt.edu/equipment -->
 * **Find and watch** any tutorials you need to begin getting a handle on Audacity
 * Be ready to share one Audacity move with your classmates
 
* **Outputs**
 * **Record** at least one spoken track to begin working with, knowing you can revise, retake, dub in, change your mind, etc.
 * **Take notes** about what kinds of other sounds you might want to add
 * **Save and commit** to git as you go
 * **Push to GitHub** at least once, so I know you're working
  * Include at least one mp3 of the current state of the project, so I can preview
  * Include your *.aup project file and *.au subdirectory, so I can try to clone and open, and so that you have a matched backup. Now that you're using git-lfs, it shouldn't lead to terrible slowdowns.
 


 


