# Website Update Instructions — dariswilson-site/index.html

These are the changes to make to `index.html`. Three categories: bio corrections, timeline corrections, and adding Issue 003 to the archive.

---

## 1. Bio Correction — Story Section

In the story section paragraph (the one starting "My name is Daris"), find:

```
I went from All-Conference D1 athlete to accountant to the NYSE trading floor to full-time entrepreneur
```

Replace with:

```
I went from All-Conference D1 athlete to accountant to the regulation side of the NYSE to full-time entrepreneur
```

---

## 2. Timeline Corrections

### 2005 entry

Find:

```
started my career on the trading floor at the New York Stock Exchange
```

Replace with:

```
started my career on the regulation side of the New York Stock Exchange
```

### 2008 entry — no changes needed.

### 2010 entry

Find:

```
Left the NYSE on March 9, 2010. Sat down at a Starbucks on Grove Street the next morning and went all in on the business. That morning is the reason this newsletter launches on March 10.
```

Replace with:

```
Left the NYSE on March 9, 2010. I had clients, but I sat down at a Starbucks on Grove Street the next morning with no safety net and started building the business around them. That morning is the reason this newsletter launches on March 10.
```

---

## 3. Add Issue 003 to the Newsletter Archive

In the `archive-grid` div, add a new card ABOVE the Issue 002 card (newest issue first). The new card:

```html
<div class="archive-card" onclick="showArticle('issue-003')">
  <p class="archive-card-meta">Issue 003 &middot; March 24, 2026 &middot; 4 min read</p>
  <h3>Every Coach Did It Differently</h3>
  <p>Discretion is the absence of systems. How one document turned six different session experiences into one consistent brand.</p>
  <span class="read-link">Read &rarr;</span>
</div>
```

---

## 4. Add Issue 003 Article View

Add a new article view div AFTER the Issue 002 article view div and BEFORE the footer. Use the same structure as Issues 001 and 002.

```html
<!-- Issue 003 -->
<div class="article-view" id="issue-003">
  <a class="article-back" onclick="showHome(); return false;">&larr; Back to Archive</a>
  <p class="article-meta">Issue 003 &middot; March 24, 2026 &middot; 4 min read</p>
  <h1>Every Coach Did It Differently</h1>

  <span class="article-section-label">From the Floor</span>
  <p>When I ran JCF Boot Camp in Jersey City, I had a team of coaches. Good ones. They cared about the members, they showed up on time, and they brought real energy to every session.</p>
  <p>But every single one of them ran sessions differently. One opened the huddle with a pep talk. Another skipped it and went straight into the demo. One did a full breakdown at the end with detailed coaching notes, another wrapped with a quick high-five and sent everyone home. The members noticed. Some loved Tuesdays and dreaded Thursdays, not because of the workout but because the experience felt like a different gym depending on who was leading.</p>
  <p>I was frustrated at first. I thought I had a coaching problem. Then I realized I had a systems problem. I had never written down what a JCF session actually looked like from start to finish.</p>
  <p>So I built what I called the Anatomy of a JCF Session. One page. It defined the structure every coach followed:</p>
  <p>Members warm up on their own before the session starts. Huddle at the top to set the intention and prime the session, ending with the "Better Body. Better Life." breakdown. Demo. Pre-workout. Main workout. Finisher. Cool down with announcements. Post breakdown: "All day. Everyday."</p>
  <p>That was it. No script for what to say during the huddle, no requirement that every coach sound like me. The structure was the standard. The personality on top of it was theirs.</p>
  <p>The moment that document existed, the member experience became recognizable no matter who was leading. Tuesdays felt like JCF. Thursdays felt like JCF. Because it wasn't the Daris way anymore. It was the JCF way.</p>

  <span class="article-section-label">The System</span>
  <p>Discretion is the absence of systems.</p>
  <p>Every place in your business where a team member is using their own judgment to fill a gap is a place where you haven't built a system yet. That's not a criticism of the person. Their judgment is often reasonable, sometimes good. But it's inconsistent by definition, because judgment varies from person to person and from day to day, and the client experience shifts with it.</p>
  <p>My coaches weren't doing anything wrong. They were doing what every capable person does when the instructions are vague: they improvised. And improvisation across a team produces variety, not consistency.</p>
  <p>This is the part most service business owners resist, because it feels like building a standard removes the personal touch. It doesn't. It protects it. When the structure is consistent, the personality on top of it has room to breathe. When the structure is missing, the personality is doing all the work, and the experience depends entirely on which team member shows up that day.</p>
  <p>The Anatomy of a JCF Session didn't tell coaches what to say or how to coach. It told them what the session looks like, the order of events, the bookends, the non-negotiable touchpoints. Within that structure, every coach brought their own style and their own energy, and the members got the benefit of both: a consistent experience and a human one.</p>
  <p>The question worth sitting with is not "is my team doing it wrong." The question is "have I defined what the experience should feel like in a way that doesn't depend on me being in the room."</p>
  <p>If the answer is no, your team is operating on discretion. And discretion, across a team, produces exactly what you're seeing: inconsistency that feels like a people problem but is actually an infrastructure problem.</p>
  <p>The standard doesn't belong to you. It belongs to the company. When you build it that way, the company can hold it whether you're there or not.</p>

  <span class="article-section-label">In My Stack</span>
  <p>I've been using Notion as the home base for all of the system documents in my coaching practice. One workspace, one template, every system linked to the others. The thing I like about it is that the documents are alive. I can update a process in two minutes and everyone with access sees the current version immediately. No emailing updated PDFs, no "which version is the latest" conversations. If you're still storing your operating documents in scattered Google Docs or text threads, try consolidating them into one workspace. The clarity of having everything in one place is worth the afternoon it takes to set up.</p>

  <div class="ask-box">
    <p>If you pulled three different team members aside and asked each one to walk you through how they handle the same client-facing task, would you hear three versions of the same answer or three completely different answers.</p>
  </div>

  <span class="article-section-label">One Thing This Week</span>
  <div class="one-thing">
    <p>Pick one client-facing experience your team delivers regularly. Write down three things: what the experience should look like from start to finish, which moments are non-negotiable, and what the client should walk away feeling. That's not a full system document. That's the anatomy of your version of a session, and it's the foundation the document gets built from.</p>
  </div>

  <div class="sign-off">
    <p>Daris</p>
    <p>Founder, From The Floor Up &middot; <a href="https://fromthefloorup.co" target="_blank" style="color: var(--strike);">fromthefloorup.co</a></p>
  </div>
</div>
```

---

## Summary of all changes

1. Two "trading floor" references changed to "regulation side" (story paragraph + 2005 timeline)
2. 2010 timeline updated to reflect Daris had clients when he left the NYSE
3. Issue 003 archive card added (above Issue 002)
4. Issue 003 full article view added (after Issue 002 article view, before footer)
