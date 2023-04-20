# Last day of class! Looking back and looking forward

**Work to have done**:

* _(Optional)_ Identify something said, read, or made in this course that you want to remember beyond this semester.
* Consider what earlier reflections,  feedback, commit messages, etc you'll want to include in the final portfolio to support your introductory letter
* Otherwise proceed on your plans toward consolidating and integrating what you've learned

**Plan for the day**:

1. Gifts and Remembrances (optional)
2. OMETs, if you haven't yet (due Sat 11:59pm)
3. Notes before studio
  - Final portfolio FAQ
4. Studio
  - Set an intention
  - Exit note
5. The ends of a term


## Gifts and Remembrances (optional)
A handful of people had voted last class in favor of sharing something awesome they made and are proud of, or something awesome they appreciated from someone else in the class, for the purposes of celebrating our collective accomplishments. I heartily support this volunteerism!

Let's take 2-3 minutes for each share, up to a total of about 10 minutes (to preserve working time for everyone who voted to work).

## About OMETs (5 min intro + 10 min to fill out)

OMETs are a pretty important way of getting your voices heard; they can also have some pretty outsized effects on your teachers' lives.

<details><summary>Expand to read more.</summary>

I know some of you have already turned in your surveys for the Office of Measurement and Evaluation of Teaching (yep, that's what OMET stands for). If so, you can feel free to work on your own projects, though I hope what I'm about to say is still useful information.

Actually, I hope you all know this stuff already, but my experience has been otherwise, so I try to say it in every class:

<div class="alert alert-info">
These evaluations of teaching serve multiple purposes, and go to multiple audiences:
<ul>
<li>They'll go to my program director, to help determine if I should keep teaching this course;</li>
<li>they'll become part of my portfolio application for promotion, read by other faculty inside and outside my department; <!-- again: renewal. also: promotion --></li>
<li>and, after grades are turned in, they'll go to me, so I can use them to revise and update the course. For that purpose, I especially value the free responses. (I also added a few Likert questions that are particular to this section of the course.)</li>
</ul>
</div>

The same is true for all your professors. For adjunct professors, OMET reviews may make the difference in whether they get renewed again at all.

So the OMETs are, as I said above, a pretty important way of getting your voices heard, which is a good thing; on the other hand, they can also powerfully affect hiring, especially for women, immigrants, and people of color.
</details>

In brief: please do fill these out, but <strong>please do your best to be fair, to be thoughtful, and to be considerate of how things like race, gender, and linguistic difference might color your responses.</strong> (Implicit biases can often be countered by bringing them to consciousness.)

<div class="alert alert-success">
If you haven't yet filled out your survey, please do so now. You should have a link to the survey on Canvas, or in your Pitt email.</div>

EXT 1: I know some of you may already have filled out the end-of-semester version of the <a href="https://bit.ly/tech-comfort-redux">Tech Comfort Survey</a>, but if you haven't, I hope you'll consider doing so now.

EXT 2: If you've done the Survey and the OMET to your satisfaction and you're waiting for your classmates to finish, you can use this time for solo work on your portfolio / revisions or your final reflection.

<!-- <div class="alert alert-white">
I'll turn off the Zoom recording and absent myself for a bit in a breakout room, just in case you want to talk amongst yourselves. Figure it'll take around 10 minutes? I'll monitor the completion rate to know when it's safe for me to come back. Or come find me if everyone's done.
</div> -->

## Notes before Studio

We'll spend just about the rest of class working on your individual and group projects / final reflections.

### Final portfolio FAQ

Some people have historically asked  questions that maybe you have floating around in your head, too.

<details><summary>What do you mean by “linked thumbnail”?</summary>

<p>All I mean by <em>thumbnail</em> is a small picture; all I mean by <em>linked</em> is that it should be clickable, a hyperlink.</p>

<p>As you know from previous reflections, you can upload an image into your post on the Issue Queue just by dragging and dropping the file, which will generate some markup like this:</p>

<div class="language-markdown highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="p">![</span><span class="nv">name-of-file.png</span><span class="p">](</span><span class="sx">https://somecrazylongURLthatGitHubauto-generates</span><span class="p">)</span>
</code></pre></div></div>

<p>If you want the image to link directly to your repository for that project, you would add another layer of markup, using the structure <code class="language-plaintext highlighter-rouge">[anchor](URL)</code>. So in this case, because the anchor is that whole long thing GitHub generated after the drag-and-drop, you’d link like this:</p>

<div class="language-markdown highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="p">[</span><span class="nv">![name-of-file.png</span><span class="p">](</span><span class="sx">https://somecrazylongURLthatGitHubauto-generates</span><span class="p">)</span>](https://github.com/username/repo)
</code></pre></div></div>

<p>Note the double closing in the middle: close-parenthesis, close-bracket. You can also use real HTML (i.e. <code>&lt;a&gt;</code>) inside Markdown, but you can't use Markdown inside HTML, so you'd need to convert the Markdown image syntax to your usual <code>&lt;img&gt;</code> syntax.</p>

<p>If that’s too annoying, you can also just paste the regular link underneath the image, like this:</p>

<pre><code class="language-Markdown">**Soundscape thumbnail:**

![name-of-file.png](https://somecrazylongURLthatGitHubauto-generates]

[Link to soundscape file](https://github.com/username/repo/blob/master/name-of-playable-file.mp3)
[Link to soundscape repository](https://github.com/username/repo)
</code></pre>

<!-- <p>Or, you know, just use real HTML: <code>&lt;a href="https://github.com/username/repo/blob/master/name-of-playable-file.mp3"&gt;&lt;img src="https://somecrazylongURLthatGitHubauto-generates" alt="thumbnail of audio project"&gt;&lt;/a&gt;</code></p> -->
</details>
<details><summary>Why do I need to link to the project <strong>and</strong> link to the repository? Aren't those the same?</summary>
<p>The project link should take us to the final, rendered version: the "flat" export, or the home page of the website. This is to avoid any potential confusion in your file structure, where it might be unclear which version is really the final one. So click through to the actual file in your repo, and then grab <em>that</em> URL.</p>
<p>That said, I also want to have easy access to the repository as a whole, so I can look at things like the README, credits, commit history, etc.</p>
</details>
<details><summary>When you say, "link to a specific point in the revision history..."</summary>
<p><strong>When I ask you to link to a specific point in the revision history</strong>, i.e. for an earlier draft, you can follow the same setup as above. That is, you can use the structure <code class="language-plaintext highlighter-rouge">[anchor](URL)</code>.</p>
<p>But instead of getting the URL of the repo as a whole, <em>click through to the commit history, like you did for workshop, and grab the URL of the commit</em> that represents that past moment you want to compare to the present.</p>

<p>Hope that clarifies things!</p>

</details>

Anything else you're wondering?


### Set an intention

As usual, please...

1. Write your goals [in the google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.1tqhsvrbsrr2)
2. Expect to leave an exit note to report on progress and re-set goals for moving forward.
3. Save an extra couple of minutes at the end of class, to bring us back together, for closure.

For Zoomers, I'll once again set breakout rooms for maximum flexibility, and otherwise hang out in the main room unless people need one-on-one time (when we can go to an extra room set aside for that purpose).

Just for fun: Final stats for the shared google doc, as of last night (and probably longer now!)
* 12,562 words
* ~40 pages
* 30,309 revisions


### Exit note

When we're getting toward those last few minutes, please head back to the google doc to write an update: What have you achieved today? What are your goals for the weekend? For the final portfolio?

## The ends of a term

* The final portfolio will be due during our final exam slot, which is **Tuesday, April 25th**. I messed up the time initially, so I'm just saying you have until the end of the day.
* The reflection is the main thing, so **if you do make revisions to earlier projects, please be sure to talk about them in the reflection.** Or even if you don’t have time to make revisions, but want to talk about what you _would_ revise, if you had more time, you can talk about that in the reflection, too. I'm most interested in what you've learned this semester, and what will help you keep learning after it ends.

* Office hour update: I have office hours today and on Tuesday at the usual 2:30-3:30, on Zoom only: <a href="https://pitt.zoom.us/my/benmiller314">pitt.zoom.us/my/benmiller314</a>. Let me know if you're coming at benmiller314.youcanbook.me, or just drop by.You can also always email me with questions.

<div class="alert alert-white">I like to <a href="https://www.poetryfoundation.org/poems/47785/at-the-san-francisco-airport">end with poetry</a>.</div>
