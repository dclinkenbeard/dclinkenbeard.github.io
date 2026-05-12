---
layout: post
title: "What Should a 300-Level Software Design Course Look Like Now?"
date: 2026-05-12 13:00
description: A working paper that asks what computer science is, what CS education should be in the era of generative AI, and what the course learning outcomes for CST 338 at CSUMB should become. Sharing a v0.1 draft for colleague review.
tags: cs-education pedagogy course-design genai software-design csumb
categories: teaching scholarship cs-education
---

_Working draft. Sharing early because I want pushback._

I just finished a working-paper draft on the foundations of my **CST 338 (Software Design)** redesign at CSUMB. It is up on GitHub for colleague review:

> **Repo:** [github.com/dclinkenbeard/cst338-redesign-foundations](https://github.com/dclinkenbeard/cst338-redesign-foundations)
> **Citable version:** [v0.1 release](https://github.com/dclinkenbeard/cst338-redesign-foundations/releases/tag/v0.1)
> **License:** CC BY-NC-SA 4.0

If you only have five minutes, read Section 1 (Working Hypothesis), Section 5 (Proposed CLO Architecture), and Section 6 (Pedagogical Commitments). Those are the load-bearing parts. The rest is the literature scan that supports them.

## What I Was Trying to Do

CST 338 is a required 300-level course in CSUMB's Computer Science major. The current Course Learning Outcomes were written before ChatGPT, before Copilot, and before the field's center of gravity shifted from "should we let students use AI?" to "we have to integrate AI; what does that mean for what we teach?"

I am redesigning the course for Fall 2026. Before I touched a single assignment, I wanted to do the boring-but-necessary work first: build an evidence base. Read the canonical CS-education literature. Read the post-2022 generative-AI literature. Write down what I actually believe, with citations, and let colleagues poke holes in it.

So I did. Then I treated the result like the outline of a meta-analysis: working hypothesis, search method, findings by theme, synthesis, implications for the course, limitations.

## The Working Hypothesis

In one sentence:

> **Generative AI does not eliminate the need for programming instruction; it relocates the cognitive bottleneck from syntax production to specification, code reading, debugging, and design critique. A 300-level software design course is precisely where students are old enough and have enough prior code experience to do the relocated work, and young enough that the habits formed here will define their professional practice.**

This is testable. If three semesters of evidence show students using LLMs to bypass design thinking entirely, the hypothesis is wrong and a different intervention is needed.

## What the Literature Actually Says

Four threads carry most of the argument.

**Foundations.** The field has spent two decades converging on a competency-based curriculum (CC2020), Peter Denning's "great principles of computing," and Jeannette Wing's computational thinking as a general literacy. The pedagogical implication: course outcomes should be competencies (knowledge + skill + disposition + task), not knowledge inventories.

**How students actually learn OOP.** Lister et al. (2004) showed that many CS1 and CS2 completers cannot reliably trace small pieces of code, which predicts they cannot design code either. Hadar and Leron (2008) showed that even experienced developers default to procedural decomposition under load: object-oriented design is counterintuitive, full stop. Caspersen and Bennedsen (2007) showed that scaffolded, modeled, faded instruction (cognitive apprenticeship) outperforms blank-page assignment design. Sanders et al. (2012) gave us the language of "threshold concepts": OOP is one, polymorphism is one, design patterns sit at one.

**Generative AI in CS education.** Finnie-Ansley et al. (2022) was the first systematic benchmark of Codex on CS1 exam questions. Codex beat the median student. Becker et al. (2023) drew the consequence in their SIGCSE position paper: the discipline has to decide quickly. Prather et al. (2023), an ITiCSE working group, reviewed 71 papers and surveyed students and instructors in twenty countries: the field is converging on relocation, not retreat. Lau and Guo (2023) captured the instructor shift in real time, "From 'Ban It Till We Understand It' to 'Resistance Is Futile.'" Vadaparty et al. (2024) showed that a whole-CS1 redesign around LLM-assisted programming is possible and produces comparable outcomes. Denny et al. (2024) in CACM is the field's current synthesis.

**Outcomes and assessment.** Fuller et al. (2007) is the canonical "Bloom for CS" paper; the CCECC's 2023 *Bloom's for Computing* gives a verb list per Bloom level. Whalley et al. (2006) is the reference for using SOLO to grade the quality of an answer, which matters more when the artifact alone is no longer diagnostic.

## What I Am Proposing for CST 338

The current syllabus has four CLOs: OO design, Java fluency, Android, and "using LLMs to assist in code creation." I argue the current CLO2 and CLO1 overlap awkwardly, the Android CLO is misaligned with what the course actually delivers, and the LLM CLO is genuinely novel but radically under-specified.

I propose four cleaner competency-form CLOs:

1. **Object-Oriented Design.** Design a multi-class Java program that applies encapsulation, abstraction, inheritance, and polymorphism appropriately, and justify each design choice in terms of the problem requirements.
2. **Software Construction in Java.** Construct, test, and document Java programs using the professional toolchain (Gradle, JUnit 5, Git, IDE), and debug them with tests, the debugger, and code reading.
3. **Design Patterns and Software Lifecycle.** Recognize when a Gang-of-Four pattern is applicable, apply it in Java/JavaFX, and discuss trade-offs against alternatives; describe at least two software development process models and identify where each is appropriate.
4. **Using Generative AI Responsibly in Software Design.** Identify when LLM assistance is appropriate, construct effective prompts that decompose a problem into LLM-tractable subtasks, read and test and critique LLM-generated code, and articulate the academic-integrity and professional-ethics considerations.

Each is mapped to ABET CAC student outcomes, traced to specific citations in the bibliography, and pinned to a Bloom level. The Android CLO is retired (or moved to an elective). Java becomes the substrate, not a separate outcome.

## Six Pedagogical Commitments That Follow

1. **Live coding and worked examples** before students are asked to produce.
2. **Code reading on day one**, before any class-hierarchy authoring.
3. **Explicit threshold-concept signposting**: when we hit encapsulation, abstraction, polymorphism, or design patterns, the lecture names the transition and previews the disorientation that usually comes with it.
4. **AI-collaboration logs** on every major assignment: a paragraph from the student stating how AI was used and how the output was verified.
5. **Bloom-verb CLOs** and a published assessment-to-CLO map.
6. **Studio-style design critique** with the critique itself graded, not just the artifact.

## What I Want From You

If you are a CS-education colleague, a CSUMB program-coordinator-adjacent reader, or a CS-ed researcher who has done this work longer than I have, three asks:

1. **Where is the literature scan thin?** Equity and identity in CS classrooms (Margolis, Fisher, et al.) is the obvious gap and I am committed to adding it in v0.2. What else?
2. **Where does the proposed CLO architecture break?** I argue for retiring the Android CLO. Is that the right call? Am I asking too much of CLO4?
3. **Where is the GenAI evidence base actually shakier than my draft makes it sound?** This is the part of the literature I trust least; it is moving fast and most of the strong claims have weeker-than-ideal sample sizes behind them.

Open an issue on the repo, drop me an email at <dclinkenbeard@csumb.edu>, or grab me at the next [SIGCSE-affiliated thing you find yourself at](https://sigcse.org/).

## Status

This is v0.1. Working draft. Not peer-reviewed. Cite as a working paper if you must, but cite the tagged release ([v0.1](https://github.com/dclinkenbeard/cst338-redesign-foundations/releases/tag/v0.1)) so the version is stable.

The next planned revision (v0.2) will incorporate the 2025 ITiCSE working-group report (*The Rest of the Robots: Generative AI in Post-Introductory Computing Education*), the equity-and-identity literature I omitted in v0.1, and any colleague feedback that lands between now and the next refresh.

---

_This draft was prepared with substantial assistance from large-language-model tools (Claude). The literature scan and source verification were performed under my direction; every citation was verified against publisher records before inclusion. The working hypothesis, the proposed CLO architecture, and the pedagogical commitments are my own argument, informed by the cited literature. The acknowledgment is in the repo's README too._
