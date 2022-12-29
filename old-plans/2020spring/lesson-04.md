



# Sound, Space, and Audacity

**Texts to have listened to:** ["Coffee Shop Conversations"](http://dmap.pitt.edu/node/248), ["Day In: Day Out"](http://dmap.pitt.edu/node/177), ["A Haunted Halt"](http://dmap.pitt.edu/node/295), ["Expedition to Planets Unknown"](http://dmap.pitt.edu/node/178), _[Breaking Bad]({{site.github_url}}/assets/sound/bb-pilot-opening.mp3)_, _[Battlestar Galactica]({{site.github_url}}/assets/sound/bg-pilot-opening.mp3)_.

**Work to have achieved:**

* Post [on the issue queue]({{site.github.issues_url}}/2) about what you noticed while listening
* Download or update [Audacity](https://www.audacityteam.org/download/)

## Plan for the day

1. Sound and space (10-15 min)
2. Audacity Demo (10-15 min)
3. Audacity Play Time (20-25 min) <!-- needs at least 30 -->
4. Share and Enjoy (10 min)
5. HW Preview (5 min)
6. Offline sketching (10 min) <!-- we ended up having only five minutes. Ten would, yes, be better -->

## 0. GitHub followup!
After last class, An asked a great and important question: what did I do in GitHub Desktop to make it aware that I was changing a file?

The answer is: nothing. I just had to change the file, and save.

As soon as that file change is saved in the repository folder, either Git or GitHub Desktop will immediately know what's up. GH Desktop will even show you the differences, if it can. It's pretty sweet!


## 1. Sound and Space: Takeaways from listening (10 min) <!-- aim to end by 2:45...?-->
<!--_notes from forum posts will go here in the morning_

<!-- Be sure to talk about layers within the clips: how might you group the sounds you heard? -->

Lots of great comments on the forum: stuff about layers, about background/foreground, about silence and volume. Let's hear some more highlights!

Key concepts:
* contrast (draws attention)
* continuity (conveys place and time)


## 2a. Audacity: getting files (5-10 min)

We're all going to work with the same materials: a couple of spoken tracks I pulled off of C-Span and a couple of instrumental tracks I found on [CCmixter](http://dig.ccmixter.org/). I'll do a quick walkthrough of some basic editing features in Audacity, then we'll play around solo for a little bit and see what we can make, even in just a few minutes!

I've updated the soundscape2020spring repository with a new folder, "in-class-exercise," that contains the following source materials. You should be able to **pull** them into your forked repo!

<details>
<summary>Show the GH Desktop screenshots, please!</summary>
<ol>
  <li><figure><img src="../assets/img/gh-desktop--merge-upstream-master-1.png" alt="select the branch menu" /></figure></li>
  <li><figure><img src="../assets/img/gh-desktop--merge-upstream-master-2.png" alt="choose a branch to merge into master" /></figure></li>
  <li><figure><img src="../assets/img/gh-desktop--merge-upstream-master-3.png" alt="choose the upstream/master branch" /></figure></li>
</ol>
</details>

<details>
<summary>Wait, can't I see what I'm merging before I merge?!</summary>

Good point! Weirdly, GH Desktop doesn't seem to be letting me. But you can also do this operation on the GitHub website, which will include a preview:

<ol>
  <li><figure><img src="../assets/img/gh-website--merge-upstream-master-1.png" alt="select the branch menu" /></figure></li>
  <li><figure><img src="../assets/img/gh-website--merge-upstream-master-2.png" alt="choose a branch to merge into master" /></figure></li>
  <li><figure><img src="../assets/img/gh-website--merge-upstream-master-3.png" alt="choose the upstream/master branch" /></figure></li>
</ol>
</details>

And if that's not working, just head on over to [github.com/benmiller314/soundscape2020spring](https://github.com/benmiller314/soundscape2020spring), click into the in-class-exercise folder, and right-click to download.

<div class="alert alert-success">
I'll run around helping anyone who needs it! While I'm doing that, <strong>if you've succeeded in downloading the files, give them a listen!</strong>
</div>

* <div class="attribution-block">Two clips from C-Span in which <a href="https://www.c-span.org/video/?c4840911/senate-leaders-speak-house-impeaches-president-trump">Senate leaders Mitch McConnell (R-KY) and Chuck Schumer (D-NY) speak immediately after the House's impeachment of President Trump.</a> Used under Public Domain, in keeping with <a href="https://www.c-span.org/about/copyrightsAndLicensing/">C-Span policies</a>. Clips extracted using Audacity and <a href="https://github.com/mattingalls/Soundflower">Soundflower</a> (by Matt Ingalls).</div>

* <div class="attribution-block"><a href="http://dig.ccmixter.org/files/JeffSpeed68/60519">The Mellotron</a> by Stefan Kartenberg (c) copyright 2019 Licensed under a Creative Commons <a href="http://creativecommons.org/licenses/by-nc/3.0/">Attribution Noncommercial  (3.0)</a> license. Ft: Javolenus</div>

* <div class="attribution-block"><a href="http://dig.ccmixter.org/files/speck/60468">Near What's True</a> by Speck (c) copyright 2019 Licensed under a Creative Commons <a href="http://creativecommons.org/licenses/by-nc/3.0/">Attribution Noncommercial  (3.0)</a> license. Ft: Apoxode</div>

* <div class="attribution-block"><a href="http://dig.ccmixter.org/files/texasradiofish/60632">The Radiant Light Orchestra</a> by texasradiofish (c) copyright 2019 Licensed under a Creative Commons <a href="http://creativecommons.org/licenses/by-nc/3.0/">Attribution Noncommercial  (3.0)</a> license. Ft: fluffy, debbizo, GeeArtriasRose, Apoxode</div>

* <div class="attribution-block"><a href="http://dig.ccmixter.org/files/airtone/60674">reNovation</a> by airtone (c) copyright 2019 Licensed under a Creative Commons <a href="http://creativecommons.org/licenses/by/3.0/">Attribution (3.0)</a> license. </div>

* <div class="attribution-block"><a href="http://dig.ccmixter.org/files/septahelix/60779">Babylonian Time Cube</a> by septahelix (c) copyright 2019 Licensed under a Creative Commons <a href="http://creativecommons.org/licenses/by-nc/3.0/">Attribution Noncommercial  (3.0)</a> license. Ft: speck, 7OOP3D, Apoxode</div>

## 2b. Audacity Demo: working with files (10 min)

<div class="alert alert-info">
A more substantial introduction is available at the <a href="http://manual.audacityteam.org/man/audacity_tour_guide.html">Audacity Tour Guide</a>, so please review that if you find yourself stuck! (Google is also your friend, of course.)
</div>

### Import. Tracks.
Visual rendering of sound.

### Select tool; zoom tool.
Play a loop. Zoom. Selection adjust. Add label at selection.

### Time shift tool.
Split vs. split new. Mute/solo tracks.

### Copy/Paste.
Works like you'd expect it should.

### Effects.
There are lots. Some good ones to start with: Fade in / out; change tempo; auto duck.

## 3. Audacity Play Time (20 min)

Your turn! Play around with the impact of different musical selections and alignments. Try splitting the speech at the pauses to extract individual words.

(NB: we can have some fun with reordering the words, but please don't push those to GitHub: we don't need any more fake news circulating!)


## 4. Share and Enjoy (10 min)

Let's hear a few! Anybody have a clip they're excited to share?

## 5. HW Preview (5 min)

## 6. Offline sketching (10 min)
I'd like to end today's class with some writing – some listing and looping – as a way to get your ideas flowing.

- In what places (physical, virtual, or imaginary) could you anchor your soundscape? Make a list. Anything you're forgetting?

- Choosing one item from your list you could work with for now, ask yourself: What kinds of stories happen there, and which of them could you reasonably tell within a few minutes?

- How can you represent that environment sonically?

- What sounds are relatively stable, or sustained, and what is incidental?

- What structures or sequences could help a listening audience follow the story?

## EXT: Soundwalk
I'm sad to say, I realized in planning today's lesson that I had to sacrifice the walkabout I had hoped to fit in. If anyone wants to try on your own or in small groups, here's a route:

<details>
<summary>Click to expand</summary>
<ol>
<li>From this room, walk around to the either stairwell by the elevators. They go up. Linger for a minute or so, then go down to floor two.</li>
<li>Circle around the second floor to the central corridor, and near the bathroom take the winding stairs down in to the Common room. Linger again.</li>
<li>Walk out toward the Heinz Chapel, across the grass, and into the chapel itself. Sit in the pews.</li>
<li>Exit the chapel and walk along Bellefield to Forbes Avenue. Cross and make a left, walking down to the fountain in front of the Carnegie Museum of Art.</li>
<li>Enter the museum, and look at the menu for the cafe for a while. Order something, if you want.</li>
<li>Step back outside, walking down Forbes toward Hillman Library, but stop at the first bus stop you meet until a bus arrives and departs.</li>
<li>Cross the street toward the Cathedral, and go past the Stephen Foster archive to the Cathedral. You'll enter on the basement, near the Cafe.</li>
<li>Listen near the elevators for a while. Then go home (or to another preferred destination) and write about what you heard.</li>
</ol>
</details>

# HW for next time:
<div class="alert alert-success">
The main writing assignment for Tuesday is to <strong>post a proposal for your soundscape narrative</strong>, including a preliminary chart of sound assets you might want to include.
</div>

There's also a little reading, related to that (and to fair use / permissive licensing):

* The term "asset" comes from a reading assignment from the book _Writer/Designer_ (Ball, Sheppard, and Arola, eds). A scan of the relevant chapter is <a title="not posted to preserve the limited distribution that helps justify my fair use claim (as does my colorless copy and the limited amount copied, relative to the book)" href="https://pitt.box.com/s/xovvpta4x2tq1cs9ywr61d2g1udka8m5
">posted to Box</a>; **please read it before writing your proposal.**
   - _Optionally_, you can read through a [short four-page webcomic](https://wiki.creativecommons.org/wiki/Howitworks_Comic1) explaining how Creative Commons (CC) licenses get attached to copyrightable materials, and how easily CC materials can be included and/or remixed in further creations... with, at a minimum, attribution. The subject is covered in _Writer/Designer_, but the comic is cute.
   - _Optionally_, you can also **read** the Stanford Overview of Fair Use, which you can find in a series of four webpages beginning at [fairuse.stanford.edu/overview/fair-use/](https://fairuse.stanford.edu/overview/fair-use/). This text, despite being called an overview, will give you a more in-depth understanding of fair use than the brief introduction in _Writer/Designer_.

* As predicted last class, I'm also asking you to **read** the following advice on sound recording, **listening to the embedded clips**:
  - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).
  - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (**Note the time skips she recommends**: sometimes a long clip is embedded, but not meant to be listened to in full.)

* To **post your proposal**, go to the [issue queue]({{site.github.issues_url}}) and reply to the relevant thread.
   - Note that this is an edit from the assignment: I realized last night that it makes more sense for you to be able to see each other's ideas, and bounce them off each other, than to start out isolated.
   - You can still choose to list your assets only in the repo.
   - But please do **include a link to your repository in your post**!
