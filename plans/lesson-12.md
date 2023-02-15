
# Visual Unit Criteria and Stretch Goals

**Work to have done**:

* Optionally [read]({{site.canvas_url}}/assignments/1092062) up on and maybe [play](http://www.typeconnection.com) with fonts (and if not for today, then for Tuesday)
* Work on your visual arguments, and push a _[rhetorical collage preview](https://github.com/benmiller314/visual-argument-cdm{{site.course.slugterm}}#deadlines-and-products)_ to GitHub: .xcf (or .psd) file, GIMP (or Photoshop) screenshot, and text description, plus updated list of assets/credits. Exported .png of the collage-in-progress.

**Plan for the Day**:
1. Help me make sure your files are interoperable
2. Reflective writing (5 min)
3. Refresher on visual arguments we've liked (5 min)
4. Gathering criteria (30-40 min)
5. Studio: set goals, then set out (25-35 min)
6. Exit note

## 1. Help me make sure your files are interoperable

On Tuesday, you'll be downloading and responding to each other's drafts. For that exchange, it would help me greatly if you could let me know who's working in GIMP, and who's working in Photoshop. Can you please **add your name to the appropriate list in [the google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes)**? Thanks!

## 2. Reflective writing (5 min)
<div class="alert alert-success">
In your own space – you won't have to share this unless you want to – do a little writing about your visual argument in progress. What's exciting about it? What's challenging about it? What are you unsure of?
</div>

## 3. Refresher on visual arguments we've liked (5 min)
Shift now in your writing to think about the [blog posts on rhetorical collages in the wild]({{site.github.issues_url}}/7) – or, if you haven't read through them in a while, look at them quickly now with an eye toward _what you're drawn to_ in these images: **what seems to make a visual design work well, especially for making some intervention in the world or the viewer? Jot down some notes.**

## 4. Gathering criteria (45 min)
Primed now by that writing and thinking, I'm going to ask you to get in groups and brainstorm in pursuit of baseline and aspirational criteria for this unit.

### 4a. Preamble (5 min)
There are several reasons I like this collaborative process:

* It helps keep my own expectations in the realm of what's possible, especially but not only in world altered by COVID, and so sets you up for success.
* It asks you to *talk to each other about what you value*. Sometimes you only figure out what you value by talking to other people about it – whether because someone puts words to something previously inchoate, or because you realize you disagree, or because you realize you're not alone.
* It gives you practice in *making explicit otherwise implicit criteria*. This isn't the last time you'll be asked to compose in a new genre, and only rarely will someone tell you how it's supposed to work.

So I do hope you'll talk within your groups about what's doable, what's worth doing, and what's worth trying even if it doesn't get done.

Given the goals of the unit, what should we set as our minimum criteria for full credit? What are some ways we might push beyond that minimum – not just in terms of quantity, but in terms of quality?

### 4b. Review, comment, and suggest (10 min)
Like last time, I've posted criteria from previous semesters in our [shared google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.8l9rdeqawbpw) as a starting point.

<div class="alert alert-success">
Working in groups, take 10 minutes to talk amongst yourselves about what's working, what's missing, and what you'd like to move or modify.

As you reach consensus, <strong>add comments</strong> or <strong>use the "suggestions" feature</strong> (click the pencil icon in the top right) to propose modifications or additions. Or ask questions, if you have them!
</div>

EXT: If you finish early, move on to the next section.


### 4c. Respond to each other (10-15 min)
Read through the other groups' notes, adding *collegial* replies to their comments in the margins to **upvote**, **ask questions**, or **propose modifications**.

Make sure to loop back to your own comments to see if you've picked up anything to respond to.

<div class="alert alert-warning">
ALT: If you're reading this asynchronously because you had to miss class, please also leave comments, especially with questions or suggestions. You will be held to these criteria, too, so make your voice heard!

We won't finalize them until after workshop later in the week.
</div>

EXT: If you finish early, move on to the next section.

## 5. Studio While I Synthesize (25 min)

I'll work solo to write up a clean list that reflects your consensus in the comments, while you all work solo (with groupmates on-hand for questions or other feedback) on your projects and any needed tutorials.

<div class="alert alert-success">As always when we head into studio time, please set yourself some <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.nvhvwfwarnzr">goals in the doc</a>; leave the last 5-10 minutes for an exit note; and then write that exit note on what you were able to achieve / what your next steps are, adding it to your initial goals back in the doc.</div>

<p class="text-center"><strong>Don't forget to save and commit and screenshot as you go!</strong></p>
<!--
<div class="alert alert-warning">
NB: If you're joining us asynchronously, please do add your goals and reflections to the doc whenever you're able to "do" today's lesson.
</div> -->


<!-- EXT: If you're feeling stuck in studio, check to see if you can answer questions in the doc; otherwise, use any remaining time to work on your projects and view any needed tutorials. -->

## 6. Exit note
Before you leave, please go back into the google doc and reply to your stated intention from earlier: how far did you get on your goal? What's your new task list heading into the weekend?


## For next time:
* **Work** to bring in a _full draft_: a solid attempt at a complete visual argument, ideally meeting baseline criteria. Rough edges are still welcome.
  - Remember that you don't need to change the project filename from draft to draft: Why duplicate or triplicate your file storage needs? If it's the same basic project, just further along, you can and keep track of which draft is which by describing what's new in your commit messages.
* **Continue** taking periodic screenshots and posting meaningful commit messages in Git
* By Tuesday morning, **push** the draft, with the same four parts as the preview *plus* an updated file crediting your sources and permissions/license to use them
  - NB: Your filenames should have an extension at the end, like .md (for Markdown files) or .txt (for plaintext files). These extensions tell the computer how to render the file. Without that info, GitHub will default to treating things as text, but your workshop partner's computer may just get confused and not display it at all.
  - Whether Box or GitHub, double-check that you can open your main project file: try downloading it into a different location. If it doesn't open with all the layers you'd want, try saving the project again. (You may have exported the first time: a good idea, but not really sufficient.)


<div class="alert alert-info">
  <p>NB: If you're getting an error that your *.xcf (GIMP) or *.psd file (Photoshop) is too large, you can teach git to use the lfs server for that file (or for all files of that type). </p>

  <p>All you have to do is edit the file called <strong>.gitattributes</strong> (note the period as the start of the filename) according to the instructions inside it: copy the line that begins with ".lfs-init" and, in your new copy, replace ".lfs-init" with the name of your large file. </p>

  <p>Note that you may want to use VS Code or the github.com interface to make the edit, because files starting with periods tend to be hidden. If you can't see the file there, either, you can <a href="https://github.com/benmiller314/visual-argument-{{site.course.slugterm}}/blob/master/.gitattributes">copy mine</a>. </p>

  <p>And if you've already done all that and it's still not working, add me as a collaborator to your repository, and I'll run the command that makes it re-scan for LFS objects.</p>
</div>


<!--
<div class="alert alert-danger"><strong>If you couldn't get git-lfs working</strong>, and even a zip file is too big for GitHub, <a href="https://www.technology.pitt.edu/services/cloud-collaboration-box-and-onedrive">you can use OneDrive</a> to share your files. But please still do use git to keep track of your revision choices when possible, perhaps by committing screenshots with noes. And may I suggest adding a link to your OneDrive folder in your GitHub repository's README.md?
</div>
-->
