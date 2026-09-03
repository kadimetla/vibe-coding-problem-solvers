---
marp: true
theme: automata
paginate: true
---

<!-- _class: lead dark -->
<!-- _paginate: false -->

<div class="kicker">O'Reilly Live Training</div>

# Vibe Coding for Problem Solvers

## Solving your own small problems with little apps

<p style="margin-top:28px;color:#B9AFA2;font-size:19px;">Lucas Soares · Automata Learning Lab</p>

---

![bg right:44%](img/s1-the-motion.png)

<div class="kicker">Start here</div>

## There's something you keep doing by hand.

Clicking through a folder one file at a time. Retyping the same thing into a spreadsheet.

You've done it so often you stopped noticing it.

---

<!-- _class: lead -->

<div class="kicker">The framework · use it on everything today</div>

# Notice → Ask → Look → Keep or kill

<div class="flow">
<div class="step"><h3>1 · Notice</h3><p>The motion you repeat</p></div>
<div class="arrow">→</div>
<div class="step"><h3>2 · Ask</h3><p>One plain sentence</p></div>
<div class="arrow">→</div>
<div class="step"><h3>3 · Look</h3><p>Open it, don't read it</p></div>
<div class="arrow">→</div>
<div class="step"><h3>4 · Keep or kill</h3><p>Most get killed</p></div>
</div>

<p class="center" style="margin-top:34px;color:#5A524A;font-size:18px;">Six stories. Every one is a turn of this loop.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 1 · the ask</div>

# One sentence was enough

---

![bg right:52%](img/app-pressroom.jpg)

## I wanted photos printed four to a page.

<div style="background:#221512;color:#efe9dc;border-left:4px solid #9B2C2C;border-radius:10px;padding:13px 16px;font-family:'JetBrains Mono',monospace;font-size:14.5px;line-height:1.45;margin-top:12px;">Build me a simple html app that I can use to upload a bunch of images and it will provide layouts for printing them into a pdf in grid mode or other modes</div>

<p style="margin-top:14px;">That prompt. First try. The browser's print dialog makes the PDF, so there's no library and nothing to install.</p>

<p style="margin-top:14px;font-size:20px;"><strong>Lesson:</strong> plain sentence first, clever later.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 2 · keep</div>

# The one I still use

---

![bg right:50%](img/app-quiz.png)

## I read things and forget them.

Asked for a quiz: give it a document, answer from the keyboard, get graded.

Seventeen months later it's still open. Twenty-five quizzes in the folder. Keyboard shortcuts, because clicking got annoying. A button that pushes what I got wrong into Anki.

<p style="margin-top:16px;font-size:20px;"><strong>Lesson:</strong> the keepers announce themselves. You don't decide up front.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 3 · the second tool</div>

# I built the same thing twice

---

![bg right:48%](img/app-file-triage.png)

## First: a folder of images, keep or bin.

One sitting. Full-screen photo, arrow keys to decide, one confirm at the end. Nothing deletes until you say so.

**Five weeks later** I hit the same wall with a folder of mixed PDFs, notes and CSVs.

I didn't go back to Finder. I built the harder version that renders every file type inline.

<p style="margin-top:14px;font-size:20px;"><strong>Lesson:</strong> your second tool is usually your first one, generalised.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 4 · notice</div>

# Pausing the video to type the time

---

![bg right:50%](img/app-video-notes.png)

## Watch, type a note, keep the timestamp.

By hand this is: pause, read the clock, type `14:32 —`, unpause. Every single note.

Now I type while it plays and click a note later to jump back to that second.

<p style="margin-top:16px;font-size:20px;"><strong>Lesson:</strong> the best candidates are motions so small you'd never file a ticket for them.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 5 · throw it away</div>

# A plan three other people needed

---

![bg](img/app-scotland-fit.jpg)

---

## The text is the source of truth.

<div class="two-col">
<div>

Type plain text. The map draws itself, the forecast fills in for those dates, drive times come from real roads, costs add up.

Edit a line, everything recomputes.

</div>
<div>

No API key. Free public services for maps, weather, routing and currency.

I wrote my cousins a one-page guide in Portuguese so they could edit it too.

</div>
</div>

<p style="margin-top:20px;font-size:20px;"><strong>Lesson:</strong> a document that computes beats one you keep updating by hand.</p>

---

![bg right:46%](img/s2-handing-it-over.png)

## Two weeks earlier, this was Iceland.

Same dates, same three people, a fully researched Iceland dossier.

Then the trip changed. I didn't edit it — I rebuilt it for Scotland, because rebuilding took an afternoon.

<p style="margin-top:16px;font-size:20px;"><strong>Lesson:</strong> cheap to make means cheap to throw away.</p>

---

<!-- _class: lead dark -->

<div class="kicker">Story 6 · the deep end</div>

# I ran a whole tournament on one

---

![bg right:52%](img/oly-type-a-time.jpg)

## Four teams. Seven events. A field with no wifi.

This is the entire organiser interface during an event.

**One number per person. That's it.**

<p style="margin-top:14px;">Brackets, seeding, medals and running totals all come out of these boxes.</p>

---

![bg right:52%](img/oly-ladder.jpg)

## Type the times, the ladder seeds itself.

Top two per team advance, highlighted as you type. Nobody argues about who qualified, because nobody worked it out.

<p style="margin-top:16px;">The bracket maths has real tests behind it — the one place in the whole collection where I wrote them.</p>

---

![bg right:52%](img/oly-board.jpg)

## Everyone else watched this on their phone.

A public scoreboard on the same local network, reached by scanning a QR code. It updates itself.

Records highlight automatically as they're broken.

---

<!-- _class: quote -->

> You don't know what to automate until you've watched yourself <span class="mark">fail at doing too much of it</span>.

<div class="by">The first version tried to run everything through a database of tasks. I threw it away and kept one screen.</div>

---

## This one is the deep end. You arrive here.

<div class="two-col">
<div>

### What it took
* Two days, not two hours
* A framework and a hosted database
* Tests for the bracket maths

</div>
<div>

### What stayed the same
* One annoying job done by hand
* Smallest thing that removed it
* First attempt thrown away

</div>
</div>

<p style="margin-top:24px;font-size:20px;">Teams, shirts, who brings the speaker — all still human. <strong>Lesson:</strong> automate the bottleneck, not the event.</p>

---

<!-- _class: lead dark -->

<div class="kicker">The framework, up close</div>

# Now you do it

---

![bg right:40%](img/01-instrument.png)

## 1 · Notice the motion

It's never "I should build an app." It's irritation. Mine, verbatim:

<div style="display:grid;gap:7px;margin-top:12px;">
<div style="background:#221512;color:#efe9dc;border-left:3px solid #9B2C2C;border-radius:8px;padding:8px 12px;font-family:'JetBrains Mono',monospace;font-size:13px;">without having to click them one by one</div>
<div style="background:#221512;color:#efe9dc;border-left:3px solid #9B2C2C;border-radius:8px;padding:8px 12px;font-family:'JetBrains Mono',monospace;font-size:13px;">So I don't have to go looking for the file</div>
<div style="background:#221512;color:#efe9dc;border-left:3px solid #9B2C2C;border-radius:8px;padding:8px 12px;font-family:'JetBrains Mono',monospace;font-size:13px;">so I never have to go there</div>
</div>

---

## 2 · Ask in one plain sentence

<div class="two-col">
<div>

### Say
* What goes in
* What you want to see
* What comes out at the end

</div>
<div>

### Don't say
* Which library to use
* How to structure the code
* Anything you'd have to look up

</div>
</div>

<p style="margin-top:24px;font-size:20px;">If one sentence gets you nothing, the sentence was vague. Not the model.</p>

---

## What can you even ask for?

<div class="bento" style="grid-auto-rows:112px;">
<div class="cell"><h3>Transformer</h3><p>Paste in, get out</p></div>
<div class="cell"><h3>Tuner</h3><p>Sliders, live preview</p></div>
<div class="cell"><h3>Triage deck</h3><p>One at a time, decide</p></div>
<div class="cell"><h3>Viewer</h3><p>Your data, your layout</p></div>
<div class="cell"><h3>Annotator</h3><p>Mark it up, export marks</p></div>
<div class="cell"><h3>Visualiser</h3><p>Numbers to a picture</p></div>
</div>

<p style="margin-top:20px;color:#5A524A;font-size:17px;">Six shapes cover most of it. Pick the shape, then describe your version of it.</p>

---

## 3 · Open it and look

<div class="two-col">
<div>

I don't read the code. I open the thing and use it.

When it's wrong I screenshot it and paste that back with a few words.

</div>
<div>

<div class="stat-grid" style="grid-template-columns:1fr;">
<div class="stat"><div class="num">108</div><div class="label">of my prompts in seven weeks were a pasted screenshot</div></div>
</div>

</div>
</div>

<p style="margin-top:20px;font-size:20px;">You already know what wrong looks like. That's the whole qualification.</p>

---

## Saying what's wrong, without the vocabulary

<div class="two-col">
<div>

Point at it in plain words.

*"The buttons are too far apart."*
*"When I press enter nothing happens."*
*"Make the list fill the width."*

</div>
<div>

Three words for what a page is made of:

* **HTML** — what's on the page
* **CSS** — how it looks
* **JavaScript** — what happens when you click

</div>
</div>

<p style="margin-top:22px;color:#5A524A;font-size:17px;">That's the entire technical prerequisite for today.</p>

---

![bg right:42%](img/07-promote.png)

## 4 · Keep it or kill it

<div class="two-col" style="grid-template-columns:1fr;">
<div>

**Keep** — you reached for it twice · it removed a motion you actually repeat · it runs with nothing installed

**Kill** — you had to talk yourself into using it · it needs babysitting · you've stopped opening it

</div>
</div>

<p style="margin-top:16px;font-size:19px;">Rebuilt the same thing three times? That's the signal to make it permanent.</p>

---

## Killing is the normal ending

<div style="display:grid;gap:8px;margin-top:6px;">
<div style="background:#221512;color:#efe9dc;border-left:3px solid #6B7280;border-radius:8px;padding:9px 13px;font-family:'JetBrains Mono',monospace;font-size:13.5px;">kill this app and delete it</div>
<div style="background:#221512;color:#efe9dc;border-left:3px solid #6B7280;border-radius:8px;padding:9px 13px;font-family:'JetBrains Mono',monospace;font-size:13.5px;">just kill the app for now is a bit trash</div>
<div style="background:#221512;color:#efe9dc;border-left:3px solid #6B7280;border-radius:8px;padding:9px 13px;font-family:'JetBrains Mono',monospace;font-size:13.5px;">kill the app, remove the code, i'm not using this</div>
</div>

<p style="margin-top:18px;font-size:20px;">The first one was killed four hours before the version that worked. Same idea, simpler build.</p>

---

## Before you trust it with anything real

<div class="two-col">
<div>

**Poke it**
* Add an item with a very long name
* Can you edit, not just add and delete?
* Reload. Is your data still there?

</div>
<div>

**Check where things go**
* Does it talk to the internet? To whom?
* Never paste a real key into something you'll share
* Test with fake data first

</div>
</div>

<p style="margin-top:20px;color:#5A524A;font-size:17px;">Press <strong>F12</strong> for errors. Copy the red text, paste it back, carry on.</p>

---

## Enough vs. stop and think

<div class="two-col">
<div>

### A quick look is enough
* Yours, and it runs locally
* A throwaway
* Nobody else opens it

</div>
<div>

### Slow down
* Anything public
* Other people's data
* Anything you'd hate to leak

</div>
</div>

---

<!-- _class: lead -->

<div class="kicker">Now you</div>

# Give me something you do by hand.

<p style="font-size:23px;max-width:24em;font-family:var(--font-display);margin-top:10px;">We'll build it here, together, in about fifteen minutes.</p>

<p style="margin-top:20px;color:#5A524A;font-size:17px;">No external accounts, no logins. Something you did this week.</p>

---

<!-- _class: lead dark -->
<!-- _paginate: false -->

<div class="kicker">Take this with you</div>

# Notice → Ask → Look → Keep or kill

<p style="font-size:20px;max-width:26em;margin-top:14px;color:#F0E6D8;">Name the motion you repeat. Ask in one sentence. Open it and look. Keep it only if you reach for it twice.</p>

<p style="line-height:1.9;font-size:17px;margin-top:22px;">
<a href="https://github.com/EnkrateiaLucca/vibe-coding-problem-solvers">Course materials — GitHub</a><br>
<a href="https://www.youtube.com/@automatalearninglab">YouTube — @automatalearninglab</a>
</p>
