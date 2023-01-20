# Audacity; Sound On, Sound Off

Welcome to Unit II!

**Work to have done:**

* Fork and clone the [audio narrative repository](https://github.com/benmiller314/audio-narrative-{{site.course.slugterm}}) so you have your own workspace, linked to the others
* Download [Audacity](https://www.audacityteam.org/download/) and watch a brief [introductory tutorial](https://www.youtube.com/watch?v=O1WzmigxZdM)


## Plan for the day

1. GitHub: Attack of the Clones (~10 min)
2. Into Audacity (25-35 min)
3. Share and Enjoy (5-10 min)
4. Generative writing (10 min, start no later than 1:50)
5. HW Preview (5 min)
EXT. Studio time


## 1. GitHub: attack of the clones

Last week, we saw how GitHub can let multiple people edit a file, integrate the changes, and keep track of the file's history using the GH website. But what if you want to change multiple files at once? What if you want to track history for files that aren't text, and can't be edited directly on their website?

As it turns out, most of the time, you're going to want to have a *local copy* of your project that you can *pull* down from the clouds, make your changes on your own machine, and then *push* back up with the changes and history intact.

In git-speak, that linked local copy is called a *clone*. There are some good instructions (including pictures) in the GitHub documentation: [https://help.github.com/articles/cloning-a-repository](https://help.github.com/articles/cloning-a-repository).


### 2a. Clone
Let's **practice by cloning the Audio Narrative Assignment Repo from last class – but your own fork of that project**, so you're able to submit changes to it. 

(NB: If you've lost your fork, you can find it again by clicking on either your profile or on the number of forks in the description block for [the original assignment repo](https://github.com/benmiller314/audio-narrative-{{site.course.slugterm}}). The latter will show you all the forks of the project you're viewing – useful for peer review, too! – and the former will show you all the repositories you're a member of.)

<figure>
<img src="../assets/img/github--clone-and-find-forks.png" alt="screenshot of github website description block, highlighting Code button (to clone), Forks, and Profile" />
</figure>

When given the option, choose "Open in GitHub Desktop."

### 2b. The GitHub Desktop interface

I probably zoomed through this too quickly last time:

1. How is the space laid out?
  * What can you see? What can't you see that you expected to, if anything?
2. What's given the most prominent visual focus? Secondary focus?
3. What features/tools do you have quick access to?
  * For instance, what's featured in the menu? What about the context menus (e.g. when you right-click)?
  * Do any of those tools let you find what you were missing?


Note that, unlike github.com, GH Desktop...
<ul>
<li>lets you "stage" multiple files at once and wrap them in a single commit.</li>
<li>makes it easier to undo or amend the most recent commit, especially if it's still local</li>
<li>lets you keep track of changes locally (on your own computer) before you're ready to share them with the world. You can even commit multiple times, but only "push" multiple commits all at once.</li>
</ul>

NB: If you use the command line, you can also access and activate even more features of Git than graphical interfaces allow. I'm going to drop this here, in case anyone finds they need it: [https://ohshitgit.com/](https://ohshitgit.com/) (or the more kid-friendly [https://dangitgit.com/](https://dangitgit.com/)).

For now, use the "Show in Finder" or "Show in Explorer" button to locate your local files.


## 2. Into Audacity (25-35 min)


Last time, we talked about how the simultaneous layering of sound can have a powerful impact on how it's perceived. Today, I'd like you to play around with that power!

<details><summary>A fun example, albeit in video</summary>
<p>Remember this anxious arrival?</p>

<iframe width="560" height="315" src="https://www.youtube.com/embed/7WIw4IbIwG8?start=8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p>Here it is again, remastered:</p>

<blockquote class="instagram-media" data-instgrm-captioned data-instgrm-permalink="https://www.instagram.com/p/BEZj3YMyAk_/?utm_source=ig_embed&amp;utm_campaign=loading" data-instgrm-version="14" style=" background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin: 1px; max-width:540px; min-width:326px; padding:0; width:99.375%; width:-webkit-calc(100% - 2px); width:calc(100% - 2px);"><div style="padding:16px;"> <a href="https://www.instagram.com/p/BEZj3YMyAk_/?utm_source=ig_embed&amp;utm_campaign=loading" style=" background:#FFFFFF; line-height:0; padding:0 0; text-align:center; text-decoration:none; width:100%;" target="_blank"> <div style=" display: flex; flex-direction: row; align-items: center;"> <div style="background-color: #F4F4F4; border-radius: 50%; flex-grow: 0; height: 40px; margin-right: 14px; width: 40px;"></div> <div style="display: flex; flex-direction: column; flex-grow: 1; justify-content: center;"> <div style=" background-color: #F4F4F4; border-radius: 4px; flex-grow: 0; height: 14px; margin-bottom: 6px; width: 100px;"></div> <div style=" background-color: #F4F4F4; border-radius: 4px; flex-grow: 0; height: 14px; width: 60px;"></div></div></div><div style="padding: 19% 0;"></div> <div style="display:block; height:50px; margin:0 auto 12px; width:50px;"><svg width="50px" height="50px" viewBox="0 0 60 60" version="1.1" xmlns="https://www.w3.org/2000/svg" xmlns:xlink="https://www.w3.org/1999/xlink"><g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd"><g transform="translate(-511.000000, -20.000000)" fill="#000000"><g><path d="M556.869,30.41 C554.814,30.41 553.148,32.076 553.148,34.131 C553.148,36.186 554.814,37.852 556.869,37.852 C558.924,37.852 560.59,36.186 560.59,34.131 C560.59,32.076 558.924,30.41 556.869,30.41 M541,60.657 C535.114,60.657 530.342,55.887 530.342,50 C530.342,44.114 535.114,39.342 541,39.342 C546.887,39.342 551.658,44.114 551.658,50 C551.658,55.887 546.887,60.657 541,60.657 M541,33.886 C532.1,33.886 524.886,41.1 524.886,50 C524.886,58.899 532.1,66.113 541,66.113 C549.9,66.113 557.115,58.899 557.115,50 C557.115,41.1 549.9,33.886 541,33.886 M565.378,62.101 C565.244,65.022 564.756,66.606 564.346,67.663 C563.803,69.06 563.154,70.057 562.106,71.106 C561.058,72.155 560.06,72.803 558.662,73.347 C557.607,73.757 556.021,74.244 553.102,74.378 C549.944,74.521 548.997,74.552 541,74.552 C533.003,74.552 532.056,74.521 528.898,74.378 C525.979,74.244 524.393,73.757 523.338,73.347 C521.94,72.803 520.942,72.155 519.894,71.106 C518.846,70.057 518.197,69.06 517.654,67.663 C517.244,66.606 516.755,65.022 516.623,62.101 C516.479,58.943 516.448,57.996 516.448,50 C516.448,42.003 516.479,41.056 516.623,37.899 C516.755,34.978 517.244,33.391 517.654,32.338 C518.197,30.938 518.846,29.942 519.894,28.894 C520.942,27.846 521.94,27.196 523.338,26.654 C524.393,26.244 525.979,25.756 528.898,25.623 C532.057,25.479 533.004,25.448 541,25.448 C548.997,25.448 549.943,25.479 553.102,25.623 C556.021,25.756 557.607,26.244 558.662,26.654 C560.06,27.196 561.058,27.846 562.106,28.894 C563.154,29.942 563.803,30.938 564.346,32.338 C564.756,33.391 565.244,34.978 565.378,37.899 C565.522,41.056 565.552,42.003 565.552,50 C565.552,57.996 565.522,58.943 565.378,62.101 M570.82,37.631 C570.674,34.438 570.167,32.258 569.425,30.349 C568.659,28.377 567.633,26.702 565.965,25.035 C564.297,23.368 562.623,22.342 560.652,21.575 C558.743,20.834 556.562,20.326 553.369,20.18 C550.169,20.033 549.148,20 541,20 C532.853,20 531.831,20.033 528.631,20.18 C525.438,20.326 523.257,20.834 521.349,21.575 C519.376,22.342 517.703,23.368 516.035,25.035 C514.368,26.702 513.342,28.377 512.574,30.349 C511.834,32.258 511.326,34.438 511.181,37.631 C511.035,40.831 511,41.851 511,50 C511,58.147 511.035,59.17 511.181,62.369 C511.326,65.562 511.834,67.743 512.574,69.651 C513.342,71.625 514.368,73.296 516.035,74.965 C517.703,76.634 519.376,77.658 521.349,78.425 C523.257,79.167 525.438,79.673 528.631,79.82 C531.831,79.965 532.853,80.001 541,80.001 C549.148,80.001 550.169,79.965 553.369,79.82 C556.562,79.673 558.743,79.167 560.652,78.425 C562.623,77.658 564.297,76.634 565.965,74.965 C567.633,73.296 568.659,71.625 569.425,69.651 C570.167,67.743 570.674,65.562 570.82,62.369 C570.966,59.17 571,58.147 571,50 C571,41.851 570.966,40.831 570.82,37.631"></path></g></g></g></svg></div><div style="padding-top: 8px;"> <div style=" color:#3897f0; font-family:Arial,sans-serif; font-size:14px; font-style:normal; font-weight:550; line-height:18px;">View this post on Instagram</div></div><div style="padding: 12.5% 0;"></div> <div style="display: flex; flex-direction: row; margin-bottom: 14px; align-items: center;"><div> <div style="background-color: #F4F4F4; border-radius: 50%; height: 12.5px; width: 12.5px; transform: translateX(0px) translateY(7px);"></div> <div style="background-color: #F4F4F4; height: 12.5px; transform: rotate(-45deg) translateX(3px) translateY(1px); width: 12.5px; flex-grow: 0; margin-right: 14px; margin-left: 2px;"></div> <div style="background-color: #F4F4F4; border-radius: 50%; height: 12.5px; width: 12.5px; transform: translateX(9px) translateY(-18px);"></div></div><div style="margin-left: 8px;"> <div style=" background-color: #F4F4F4; border-radius: 50%; flex-grow: 0; height: 20px; width: 20px;"></div> <div style=" width: 0; height: 0; border-top: 2px solid transparent; border-left: 6px solid #f4f4f4; border-bottom: 2px solid transparent; transform: translateX(16px) translateY(-4px) rotate(30deg)"></div></div><div style="margin-left: auto;"> <div style=" width: 0px; border-top: 8px solid #F4F4F4; border-right: 8px solid transparent; transform: translateY(16px);"></div> <div style=" background-color: #F4F4F4; flex-grow: 0; height: 12px; width: 16px; transform: translateY(-4px);"></div> <div style=" width: 0; height: 0; border-top: 8px solid #F4F4F4; border-left: 8px solid transparent; transform: translateY(-4px) translateX(8px);"></div></div></div> <div style="display: flex; flex-direction: column; flex-grow: 1; justify-content: center; margin-bottom: 24px;"> <div style=" background-color: #F4F4F4; border-radius: 4px; flex-grow: 0; height: 14px; margin-bottom: 6px; width: 224px;"></div> <div style=" background-color: #F4F4F4; border-radius: 4px; flex-grow: 0; height: 14px; width: 144px;"></div></div></a><p style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; line-height:17px; margin-bottom:0; margin-top:8px; overflow:hidden; padding:8px 0 7px; text-align:center; text-overflow:ellipsis; white-space:nowrap;"><a href="https://www.instagram.com/p/BEZj3YMyAk_/?utm_source=ig_embed&amp;utm_campaign=loading" style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; font-style:normal; font-weight:normal; line-height:17px; text-decoration:none;" target="_blank">A post shared by Star Wars Remastered® (@starwars.remastered)</a></p></div></blockquote> <script async src="//www.instagram.com/embed.js"></script>
</details>



I'll ask you all to work with the same materials, just for today. In the audio-narrative-{{site.course.slugterm}} repository that you just cloned, you'll find a folder labeled "in-class activity." That folder contains:

* A one-minute selection from President Biden's inaugural address;
* A handful of instrumental tracks I found on [CCmixter](http://dig.ccmixter.org/), a site for sharing music with explicit permission to use and (often) modify.
* The full credits for these sound files, in the file CREDITS.md.

<div class="alert alert-success">
Your task for the next 20 minutes or so is to try mixing, matching, splitting, sliding, realigning, and otherwise messing around with these tracks.
  <ol>
    <li>To get started, <strong>use File > Import > Audio...</strong> to pull in an mp3 from the in-class-activity folder.</li>
    <li>Play with the strategies from last class: how does the mood change as you change the soundtrack? The left/right mix? The alignment? The tempo?</li>
    <li>Experiment with what tools the context menus and track menus offer: what does Audacity <em>expect</em> you to want to do, based on what it makes readily available?</li>
    <li>Play with the Effects menus: some good starting points include fade in/out, repeat, change tempo, delay, low pass filter. Check the "manage" button in Effects dialog boxes to see if there are any presets to try, or the ? button to learn more about that particular effect.</li>
    <li>Try splitting the speech at moments of silence to extract individual words, using Edit > Clip Boundaries > Split (or Split New). (NB: we can also have some fun with reordering the words, but please don't push those doctored speeches to GitHub: we don't need any more fake news circulating!)</li>
    <li>etc</li>
  </ol>
</div>



<!-- I'll split the class into groups, so you can talk amongst yourselves as needed without it getting overwhelming.   -->

<!-- <div class="alert alert-info">
In general, <strong>when we're in breakout groups, I encourage you to unmute</strong> and have your cameras on – as long as your background sounds won't hog the microphone.
</div> -->

For this activity, headphones will help you isolate your Audacity playback from each other.

<!-- If/when you want to share, you can set the Audacity playback to "Zoom Audio Device," which you can do from the toolbar, as shown below. If you don't see that option, you may need to use the Transport menu to Rescan Audio Devices. 

<figure>
<img src="/{{site.course.base_path}}assets/img/audacity--output-device-3.png" alt="Selecting the output device from the toolbar. The output device defaults to "Built-in Output." />
<figcaption>By default, the output device taskbar sits just above the main track window, marked with the icon of a speaker. If you haven't changed it, it probably reads "Built-in Output."</figcaption>
</figure>

<div class="alert alert-warning">NB: If your computer can't handle both Zoom and Audacity, it's okay (not ideal, but okay) to drop out of the call for a few minutes while you're working. But do <strong>set a timer</strong>, so you can check back in after about 20 minutes.</div>
-->

<p>The <a href="https://www.youtube.com/watch?v=O1WzmigxZdM">tutorial</a> I asked you to watch for homework should have given you the overview you need to jump in and get editing, but do call me in if you have questions!</p> <!-- You can use the "Ask for Help" button (<img src="https://assets.zoom.us/images/en-us/desktop/generic/in-meeting/ask-for-help-icon.png" alt="ask for help button, which shows a question mark in a circle" class="d-inline-block" />) in your meeting menu. -->


<p>EXT?: Audacity is complex enough that I'm really expecting you can fill the time here without an EXT: there are dozens of automatic effects, each with their own options and help pages! But if you're really happy with what you've achieved, go ahead and save the project, then mute the current music and add a different soundtrack. How does that shift your perception of the edits you'd already made? What else does it make you want to try?</p>


<h2>3. Share and Enjoy (5-10 min)</h2>

<p>I'd love to hear some of these, if time allows! </p>
<!-- Set your output device as shown above to play through Zoom. -->


<h3>Side note on saving: project files vs. rendered files</h3>

<p>**Audacity project files, with extension .aup3, are not playable in any program other than Audacity.** Strictly speaking, they're not actually sound files: they're a database *of* a large number of sound files, bundled together with the files themselves, plus information about track display sizes, whether they're muted, how much they're panned left or right, and so on.</p>

<p>(In fact, until Audacity 3.x, all these files and the index of metadata used to be separate. It's a mixed bag that they're not any more: on the one hand, it's harder to mess up. On the other, it makes that unified file a lot larger.)</p>

<p><strong>To make the file playable, you have to <em>render</em> it by using File &gt; Export As.</strong> You're probably fine to use .mp3 format for most purposes.</p>

<div class="alert alert-warning">
NB: I believe it'll export the whole file, across all layers, as long as nothing's selected - but it might try to export only your selection if something *is* selected when you start the export. Something to watch out for, at any rate.
</div>

<h2>4. Generative loop writing</h2>

<p>As you know, the project proposal is due by next class; it should include some basic premise of your narrative;
some sense of setting; a link to your project repository; and a table of potential assets like the one you read about in <em>Writer/Designer</em>.</p>

<p>To help you get there, I'd like to spend the remainder of our in-class time using writing – some listing and looping – as a way to get your ideas flowing. <strong>As I ask the following questions, pause and reach out with your feelings until you sense an answer, or more than one, and then write down whatever comes.</strong> I won't collect these, so they're private to you. But I hope you'll find them useful for getting to something shareable, moving forward.</p>

<ol>
  <li><p>In the process of writing with sound, you're going to spend a big chunk of time listening and relistening and looping, so you want to pick a place you're likely to enjoy hanging out in.</p>
  <p>What <em>places</em> (physical, virtual, or imaginary) come to mind as energizing for you to unpack into layers, and reassemble? In other words: within what <em>soundscapes</em> might you anchor your narrative? <strong>Make a list.</strong> Anything you're forgetting?</li>
  <li>Choosing one item from your list you could work with for now, ask yourself: How would you represent that <em>environment</em>sonically?
    <ul>
      <li>e.g. What sounds are relatively stable, or sustained, in that place? </li>
      <li>e.g. What incidental, or foreground, sounds do you associate with that place?</li>
    </ul>
  </li>
  <li>Still in the same environment: What kinds of <em>stories</em> happen there? Again, make a list. </li>
  <li>Look over your list of stories, and ask yourself: which of these could you reasonably tell within a few minutes? which are long enough to tell <em>for</em> a few minutes?</li>
  <li>Choosing one story to work with for now – you can always come back to other items on the list over the weekend – ask yourself: 
    <ul>
      <li>What are the pieces of this story? What are the actions, structures, or sequences?</li>
      <li>How would you represent each action _for audio_? What sounds, signals, or setups could help a listening audience know what was happening?</li>
    </ul>
  </li>
</ol>


<h2>EXT: Studio time</h2>

If we have more time left in class, go ahead and start writing up your proposal – or start testing the feasibility of what you want to propose, e.g. by searching for sounds you think you'll need, or opening further Audacity tutorials.

If we get up to this step, please go to our shared notes doc, [bit.ly/cdm{{site.course.slugterm}}-notes](http://bit.ly/cdm{{site.course.slugterm}}-notes) to set your working goals for today. When we're done, you can come back to the doc and update with your progress / goals for your next working session.


## Homework for next time

* The main writing assignment for the weekend is to <strong>post a proposal for your soundscape narrative by Tuesday</strong>, including a preliminary list of sound assets you might want to include.
  - To encourage cross-pollination, I'd like you to post these **to the [issue queue]({{site.github.issues_url}})**.
  - If you're feeling stuck on what to propose, see the <a title="Because you reach for them when you feel like you're falling">"parachute prompts"</a> at the bottom of the [project assignment](https://github.com/benmiller314/audio-narrative-{{site.course.slugterm}}#parachute-prompts).

* You also have some reading, as you know:
   * If you haven't yet looked at the chapter from  _Writer/Designer_ (Ball, Sheppard, and Arola, eds) on sources and credits, **please read it before writing your proposal.** A scan of the relevant chapter is <a title="not posted to preserve the limited distribution that helps justify my fair use claim (as does my colorless copy and the limited amount copied, relative to the book)" href="{{site.canvas_url}}/assignments/849366">posted to the Perusall social annotation software on Canvas</a>.
   * I'd also like you to **read** the following advice on sound recording, **listening to the embedded clips**:
     - Fowkes, Stuart. “The Top 5 Things You Need to Make a Great Field Recording.” *Cities & Memory: Field Recordings, Sound Map, Sound Art*, 13 Aug. 2014, [https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/](https://citiesandmemory.com/2014/08/top-5-things-need-make-great-field-recording/).
     - MacAdam, Alison. “6 NPR Stories That Breathe Life into Neighborhood Scenes.” *NPR Training*, 30 Oct. 2015, [https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/](https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/). (**Note the time skips she recommends**: sometimes a long clip is embedded, but not meant to be listened to in full.)
  * Finally, I have some _optional_ further readings on Creative Commons and Fair Use. If Ball et al. struck a chord with you, here's where to read on!
    - A [short four-page webcomic](https://wiki.creativecommons.org/wiki/Howitworks_Comic1) explaining how Creative Commons (CC) licenses get attached to copyrightable materials, and how easily CC materials can be included and/or remixed in further creations... with, at a minimum, attribution. The subject is covered in _Writer/Designer_, but the comic is cute.
    - The Stanford Overview of Fair Use, which you can find in a series of four webpages beginning at [fairuse.stanford.edu/overview/fair-use/](https://fairuse.stanford.edu/overview/fair-use/). This text, despite being called an overview, is really a more in-depth understanding of fair use than the brief introduction in _Writer/Designer_.

* PS: Have you seen our plentiful <a href="{{site.github_url}}/resources">Resources</a> page? Be sure to at least skim both the free/licensed sounds and music section and the audio-unit-specific advice and examples.
