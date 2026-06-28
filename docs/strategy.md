# WhatIfAbingdon strategy

Status: working strategy
Date: 28 June 2026
Project: WhatIfAbingdon / WhatIf<City>

## 1. Strategic position

WhatIfAbingdon should begin as a lightweight public imagination experiment, not as a civic technology platform.

The project uses visual stories to help people briefly experience a plausible alternative version of a familiar place. The point is not to persuade people to support a proposal. The point is to change the quality of civic imagination by asking better questions:

> What if this place felt different?

The first version should protect the original spark: local, curious, visual, public, and alive.

It should not feel like a planning consultation, policy campaign, design system, council engagement exercise, AI art gallery, or speculative architecture portfolio.

It should feel like an intriguing local story that makes someone pause and think:

> I had not looked at this place that way before.

## 2. Core idea

**WhatIf<City>** is an open civic experiment that uses visualisations, stories, examples, and public discussion to imagine plausible alternative versions of familiar places.

It starts from the observation that every town already creates experiences. Streets, rivers, parks, squares, crossings, shopfronts, pavements, and public buildings already shape what people feel able to do.

Because those experiences become familiar, they become difficult to question.

WhatIfAbingdon makes alternative experiences temporarily visible.

It does this by creating believable glimpses of possible civic realities and asking people what they notice.

## 3. The Abingdon river example

The first story should probably be:

> What if you could swim in the Thames at Abingdon?

This works because the river already appears to promise something that everyday life does not fully allow.

Current reality:

* the river is visually beautiful
* access is limited and uneven
* water quality creates concern
* the river is psychologically treated as something not to touch
* for many people it is scenery, not civic space

Possible alternative reality:

* safe seasonal swimming
* easier access into and out of the water
* people gathering near the river
* children and families using the river as part of everyday life
* the river becoming shared civic space rather than backdrop

The interesting question is not:

> Should Abingdon build swimming steps?

The richer question is:

> What would Abingdon become if the river became part of everyday public life?

## 4. What the project is and is not

### It is

* a public imagination experiment
* a visual story site
* a way to prototype civic experiences
* a way to explore plausible alternatives
* a way to observe what kinds of conversations emerge
* a way to help people see familiar places with fresh eyes

### It is not

* a campaign
* a planning proposal
* a masterplan
* a consultation exercise
* an AI image gallery
* a speculative architecture project
* a polished civic-tech platform
* a claim that any specific idea should happen

The project should consistently avoid sounding as if it already knows the answer.

The strongest stance is:

> Here is a possible world. What do you notice?

## 5. Strategic risk: over-building too early

The main risk is not technical failure. Astro and GitHub are manageable.

The main risk is strategic drift.

The project could easily become too formal, too structured, too civic-tech, or too method-heavy before it has tested whether the original idea works.

Avoid building too much too early.

Do not start with:

* a full reusable framework
* a public method library
* a large information architecture
* extensive public documentation
* polished taxonomies
* too many content types
* excessive schema design
* pages called method, principles, references, places, or framework

Those things may become useful later, but they should not define the public MVP.

The first job is to publish one compelling story and see what happens.

## 6. Public MVP

The first public version should be deliberately small.

Recommended public site structure:

```text
/
  Home

/stories/
  What If stories

/stories/swim-in-the-thames/
  What if you could swim in the Thames?

/about/
  About the experiment
```

This is enough to test the concept.

The public site should feel like a small civic magazine, not a system.

## 7. Internal structure

The repo can still contain internal material, but it should be kept behind the curtain.

Recommended internal structure:

```text
whatifabingdon/
  public/
    images/
      stories/
      stickers/
      maps/

  src/
    content/
      stories/
      field-notes/
      sources/

    components/
      StoryCard.astro
      PullQuote.astro
      ImageFigure.astro
      QuestionBlock.astro
      TradeOffs.astro
      FieldNoteCallout.astro

    layouts/
      BaseLayout.astro
      StoryLayout.astro

    pages/
      index.astro
      about.astro
      stories/
        index.astro
        [slug].astro

    styles/
      global.css

  docs/
    editorial-notes/
      story-shape.md
      tone-of-voice.md
      visualisation-notes.md
      field-experiment-notes.md
```

The public reader should see stories. The repo can hold the method.

## 8. Public language

Avoid public labels that make the project sound institutional.

Avoid:

* case study
* framework
* method
* intervention
* stakeholder
* civic engagement
* consultation
* proposal
* design principles
* experience design analysis

Prefer:

* story
* what if
* possible future
* how it feels now
* what could be different
* what would need to be true
* what might make this hard
* what do you think?

The language should create curiosity before explanation.

## 9. Editorial strategy

The hard part is not Astro. The hard part is the writing.

Each story needs to work as an explainer, not as a design artefact.

It should have:

* a strong hook
* a familiar local place
* a clear description of how it feels now
* one vivid alternative
* examples from elsewhere
* a short explanation of why those examples matter
* visualisations treated as evidence inside the story
* practical constraints and trade-offs
* open questions for readers
* a good ending

The model is closer to Vox, The Pudding, Works in Progress, or a strong public explainer than to a local planning document.

The reader should not need to already care about urbanism, planning, design, climate, transport, or local government.

The story has to create the curiosity.

## 10. Suggested story shape

Use this as a flexible editorial pattern, not a rigid template.

1. **Hook**
   Start with a question that makes the familiar place feel newly strange.

2. **The familiar place**
   Ground the reader in something they recognise.

3. **How it feels now**
   Describe the current experience in everyday language.

4. **The what if**
   Introduce one alternative reality.

5. **One possible future**
   Use visualisations carefully. Label them as one possible future, not the future.

6. **Has anywhere done this?**
   Bring in examples from elsewhere. Do not say “copy this”. Ask what can be learned.

7. **What would need to be true?**
   Explain the enabling conditions.

8. **What might make this hard?**
   Show constraints, risks, costs, maintenance, objections, ecological questions, safety, access, and politics.

9. **What this reveals**
   Pull the story back to the experience of living in the town.

10. **What do you think?**
    End with open questions rather than a call to support or oppose.

## 11. Example: river story hook options

Possible hooks:

* Why does one of the prettiest places in Abingdon feel slightly off limits?
* The Thames might be Abingdon’s biggest missed opportunity.
* What if the river was not just something to look at?
* What if Abingdon treated the Thames as a public space, not a backdrop?
* What if you could swim in the Thames after work?

The hook should make the current reality feel visible without sounding accusatory.

## 12. The experience design lens

The deeper project is about experience design applied to towns.

But this should be revealed through the writing, not announced as professional jargon.

For internal use, each story can still include an experience design lens:

| Current experience                    | Possible alternative                     | Design principle                                                                         |
| ------------------------------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------- |
| The river is designed to be observed. | The river becomes part of everyday life. | Public places become more valuable when they invite participation, not just observation. |
| People pass through the square.       | People stay in the square.               | Civic space needs reasons to dwell, not just routes through.                             |
| Children are driven short distances.  | Children cycle independently.            | A town feels different when children can move through it safely.                         |

This can become a pattern language over time, but it should emerge from stories rather than precede them.

## 13. AI visualisation strategy

AI images are not the product.

They are a rapid prototyping medium.

Use them to help people momentarily experience an alternative civic reality.

Rules:

* never present AI images as predictions
* never imply the image is a proposal
* always explain the thinking around the image
* use captions to clarify what the image is exploring
* keep images plausible, local, and grounded
* avoid fantasy aesthetics
* avoid render-porn
* avoid making the project feel like an AI art showcase

Good caption pattern:

> One possible future: the Thames as a seasonal civic swimming space, with safer access, places to sit, and a clearer relationship between the town and the water.

Bad caption pattern:

> Proposed river swimming development.

## 14. The street experiment layer

The project should not live only online.

The physical layer is central:

* posters
* stickers
* QR codes
* short links
* small signs
* local placements near the places being discussed

The loop is:

```text
publish a story
place prompts in the town
observe what happens
capture field notes
adjust the next story
```

This preserves the project as an experiment rather than a publication machine.

## 15. Field notes model

Create lightweight field notes for real-world experiments.

Example:

```markdown
---
title: "Thames swimming QR poster test"
date: "2026-07-01"
story: "swim-in-the-thames"
locations:
  - "Near the river path"
  - "Abbey Meadows entrance"
materials:
  - "A4 poster"
  - "QR code"
  - "Short URL"
observations:
  scans: null
  comments: []
  visibleReactions: []
---

## What we tried

## Where it was placed

## What happened

## What surprised us

## What to change next time
```

Do not over-measure. Capture enough to learn.

Useful observations:

* which stories are scanned or shared
* which ideas generate comments
* which ideas annoy people
* which ideas make people tell stories
* which ideas make people say “I had never thought of that”
* which locations seem to work for physical prompts
* which framings feel too political, too vague, or too polished

## 16. Measurement approach

Success should not initially mean policy change.

Early success means the experiment improves the quality of attention, imagination, and conversation.

Look for signals such as:

* people share the story
* people discuss the place differently
* people contribute examples from elsewhere
* people raise practical objections
* people suggest smaller versions
* people disagree with the idea but engage with the question
* people say the visualisation made them notice something
* local groups, councillors, businesses, or residents ask to discuss it

The key hypothesis:

> Showing people believable alternative experiences can lead to richer civic conversations than asking abstract planning questions.

This does not need to be proven on day one. It needs to be investigated.

## 17. Content principles

### Experience before infrastructure

Focus on how places feel and what they allow people to do, not only on what they contain.

### Curiosity before certainty

Ask better questions. Avoid sounding as if the answer is already known.

### Plausibility over fantasy

The alternative should feel imaginable enough to discuss seriously.

### Story before method

The public should encounter a compelling story. The method can remain internal.

### Trade-offs before cheerleading

Every possible future has costs, constraints, risks, losers, maintenance burdens, and unintended consequences.

### Local first

The story should feel rooted in Abingdon, not imported from an urbanist playbook.

### Open ending

End with questions, not a demand.

## 18. Possible future stories

Candidate stories:

* What if you could swim in the Thames?
* What if every child could cycle safely to school?
* What if Market Place had no cars?
* What if Abbey Meadows flooded by design instead of accident?
* What if empty shops became community workshops?
* What if the high street belonged to people first?
* What if the town centre had more reasons to stay after 5pm?
* What if the river path worked for everyone?

Do not build pages for all of these yet.

Use them as a backlog, not as a promise.

## 19. Technical strategy

Use Astro and GitHub to create a small static story site.

Technical priorities:

* simple content structure
* fast pages
* accessible HTML
* easy Markdown authoring
* reusable but minimal story layout
* image captions and alt text
* lightweight field notes
* no unnecessary CMS at the start
* no early platform abstractions

Avoid heavy schema design. Let the first story teach the structure.

Recommended first collections:

```text
src/content/stories/
src/content/field-notes/
src/content/sources/
```

The first story schema should be light:

```yaml
title: "What if you could swim in the Thames?"
slug: "swim-in-the-thames"
status: "draft"
summary: "A story about whether the river could become part of everyday public life in Abingdon."
place: "The Thames"
theme:
  - river
  - public life
  - swimming
heroImage: "/images/stories/swim-in-the-thames/hero.jpg"
streetExperiment:
  qrCode: true
  posterLocation: "Near the river"
  startDate: "2026-07-01"
```

The Markdown body should carry the richness.

## 20. Deployment strategy

Do not assume GitHub Pages is automatically the right deployment target.

GitHub Pages is fine if the project should stay simple, static, public-repo-native, and free.

Netlify or Vercel may be better if deploy previews, redirects, simple forms, or easier publishing become important.

For now, the strategic priority is not hosting purity. It is keeping the publishing loop easy enough that the experiment continues.

## 21. Anti-drift guardrails

Use these checks before adding features.

### Before adding a page

Ask:

> Does a public reader need this now, or is this internal scaffolding?

### Before adding a content type

Ask:

> Have we repeated the pattern enough to know this needs structure?

### Before adding method language

Ask:

> Does this make the project more understandable, or more institutional?

### Before adding polish

Ask:

> Does this help the story land, or does it make the experiment feel less alive?

### Before calling something a framework

Ask:

> Has the method earned that name through use?

## 22. First milestone

MVP 0.1 should include:

Public:

* home page
* stories index
* one story page
* about page

Internal:

* story content folder
* field notes folder
* sources folder
* editorial notes folder
* one strategy document

First story:

* What if you could swim in the Thames at Abingdon?

First field experiment:

* one poster or sticker route with QR code near the river
* one short observation note after placement
* one revision to the story or framing based on what happened

## 23. Working summary

WhatIfAbingdon should start as a lightweight visual story experiment that asks whether imagination can become a useful civic tool.

The website is not the main product.

The main product is the moment where someone looks at a familiar place and briefly experiences it differently.

The first job is to create that moment once, clearly and compellingly.

Everything else should wait until the experiment earns it.
