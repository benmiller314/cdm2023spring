
# Parting Gifts
aka Something / That I Remember

**Texts to have read**:

* Paul Ford's <a href="https://www.nytimes.com/2019/06/11/magazine/letter-of-recommendation-bug-fixes-git.html">"Letter of Recommendation: Bug Fixes"</a>
* Your own change logs (commit histories)
* Lesson plans on this website

**Work to have done**:

* Identify something said, read, or made in this course that you want to remember beyond this semester.
* Work toward your consolidation unit project

**Plan for the Day**:

1. OMETs (and tech comfort survey, take 2)
2. Final portfolio clarification of terms
3. Consolidation projects: intros and sendoffs
4. Studio time
5. Endless departures

## 1. OMETs, then studio time

<div class="alert alert-info">
Remember that these evaluations of teaching serve multiple purposes, and go to multiple audiences:
<ul>
<li>They'll go to my program director, to help determine if I should keep teaching this course. (NB: if your other classes are being taught by adjuncts or other part-time faculty, that may make the difference in whether they get renewed again at all.)</li>
<li>They'll become part of my portfolio application for tenure, read by other faculty inside and outside my department.  <!-- again: renewal. also: promotion --></li>
<li>And, after grades are turned in, they'll go to me, so I can use them to revise and update the course. For that purpose, I especially value the free responses. (I also added a few questions that are particular to this iteration of the course.)</li>
</ul>
</div>

So the OMETs are pretty important!

<div class="alert alert-white">
If you haven't yet filled out your survey, please do so now. You should have a link to the survey on the homepage of your CourseWeb account, or in your Pitt email.

EXT: If you haven't yet, I also encourage you to head over to the <a href="http://bit.ly/cdm-tech-survey">Tech Comfort Survey</a>, then search your email for the corresponding answers you'd given in January. Fodder for your final reflection, perhaps?
</div>


## 2. Final portfolio clarification of terms

**Someone asked what I meant by "linked thumbnail":** all I mean by _thumbnail_ is a small picture; all I mean by _linked_ is that it should be clickable, a hyperlink.

As you know from previous reflections, you can upload an image into your post on the Issue Queue just by dragging and dropping the file, which will generate some markup like this:

```markdown
![name-of-file.png](https://somecrazylongURLthatGitHubauto-generates)
```

If you want the image to link directly to your repository for that project, you would add another layer of markup, using the structure `[anchor](URL)`. So in this case, because the anchor is that whole long thing GitHub generated after the drag-and-drop, you'd link like this:

```markdown
[![name-of-file.png](https://somecrazylongURLthatGitHubauto-generates)](https://github.com/username/repo)
```

Note the double closing in the middle: close-parenthesis, close-bracket.

If that's too annoying, you can also just paste the regular link underneath the image, like this:

```Markdown
**Soundscape thumbnail:**

![name-of-file.png](somecrazylongURLthatGitHubauto-generates]

[Link to soundscape file](https://github.com/username/repo/blob/master/name-of-playable-file.mp3)
[Link to soundscape repository](https://github.com/username/repo)
```

**When I ask you to link to a specific point in the revision history**, i.e. for an earlier draft, you can follow the same setup as above. But instead of getting the URL of the repo as a whole, _click through to the commit history, like you did for workshop a couple of weeks back, and grab the URL of the commit_ that represents that past moment you want to compare to the present.

Hope that clarifies things!


## 3. Consolidation projects: introductions and send-offs

I don't have a chance here to convene all of us together, as we would in a normal semester, to celebrate the work you've done: enough people have written to tell me they don't have the availability or the connectivity to make a real-time call together during our class window, and outside that window is even harder.

Still: I want you to know that I am incredibly proud of what you've produced this semester, even since the shift to online / distant learning, but really all year long.

<!--
This isn't a workshop, but rather a celebration, and an invitation: afterward, we'll have time to play through the games and scroll through the websites.

So walk us through
<ol class="lower-alpha">
<li>an introduction to the thing you made:
  <ul>
    <li>what's the premise?</li>
    <li>where can we access it? (can someone in the group write the URL on the board?)</li>
  </ul>  
</li>
<li>a celebration of group members' strengths and contributions<!--remember that from the criteria?--><!--, and</li>
<li>what the fate of the project will be for the foreseeable future:
    <ul>
        <li>will you keep it alive?</li>
        <li>can others participate if they want?</li>
    </ul>
</li>
</ol> -->

## 4. Studio time

You know how this works by now.

<div class="alert alert-success">
Before you start your solo time today, <a href="http://bit.ly/cdm2020spring-criteria#heading=h.mbz01ya98yd1">head over to the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
  <ul>
    <li>Locate tutorials (for what)?</li>
    <li>Gather assets you can use in your project?</li>
    <li>Write code, public-facing copy, something for yourself to help clarify your idea?</li>
    <li>etc etc</li>
  </ul>
Just a sentence or two as a guidepost will give you something to come back to, to reorient, if you find yourself walking in circles or caught in a thicket.
</div>

<!-- <div class="alert alert-success"> -->
Take 70 minutes, and subtract however long you just spent reading the sections above. Then give yourself reminders to stretch, save, and write commit messages as you go!
<!-- </div> -->

I'll be online [in Zoom](https://pitt.zoom.us/j/4969331343) from 2:30-3:45pm.

<div class="alert alert-warning">
Don't forget to save periodically as you go:
 <ul>
   <li>as a project file, if appropriate</li>
   <li>as a git commit, saying what you've just achieved</li>
   <li>as a screenshot</li>
 </ul>
</div>

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular CSS skill? Decide something about your project? Raise a question in a new way that you'd like some help with?

<div class="alert alert-success">
<strong>Head back into the <a href="http://bit.ly/cdm2020spring-criteria#heading=h.mbz01ya98yd1">google doc</a> and reply to your intention-post.</strong> You could email me directly if you prefer, but I'm hoping some of your insights or achievements will help inspire others.
</div>

## 5. Endless departures

And other announcements.

* If you're not yet satisfied with your consolidation project, aim to be finished with it by Sunday, so you have time to work on your final portfolio reflection.

* If we had a final exam, it would be **this coming Tuesday,** from 12:00pm-1:50pm. Instead, the [final portfolio](https://github.com/benmiller314/cdm2020spring/blob/gh-pages/uploads/handout--final-portfolio-prompt.docx?raw=true) is due to the [Issue Queue]({{site.github.issues_url}}) at the end of that exam slot: Tuesday, April 21, at 1:50pm.

* **The reflection is the main thing**, so if you do make revisions, please be sure to talk about them in the reflection. Or even if you don't have time to make revisions, but want to talk about what you *would* revise, talk about that in the reflection, too. Be sure you see the guiding questions in the handout linked above.

* Having everyone at home makes it hard to hold extra office hours, but please do email me or use the Issue Queue if you have any questions or want to see a demo of anything! If we can find a good time for a Zoom call, I'll do my best to help.

* If you're coming up on the end of the weekend and realize that a few extra days would make the difference between feeling cut off and feeling finished, just let me know! The school's given me a little extra flexibility on getting grades in, and I can certainly pass that on to you. But I also want to be mindful of not dragging the semester on longer than you can sustain.


## [We end with poetry](https://merwinconservancy.org/2019/03/now-it-is-clear-by-w-s-merwin-2/).
