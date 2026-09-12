# BA305 — The Project Proposal

**Fall 2026 · Due Thu Sep 17, 11:59 PM · One page, PDF, one per team · Worth 10% of your project grade**

> **This is a convenience handout.** Everything here is drawn from [`PROJECT_DIRECTIVES.md`](PROJECT_DIRECTIVES.md) and the course syllabus, which remain the sources of truth. Section references (§) point back into the directives, and where this page and the directives disagree, the directives are correct.
>
> *Last synced to `PROJECT_DIRECTIVES.md` and the syllabus: **2026-09-11**.*

---

## 1. At a glance

|  |  |
| --- | --- |
| **Due** | **Thu Sep 17, 11:59 PM** (Session 5) |
| **Where** | Blackboard — one submission per team |
| **Format** | **One page, PDF.** Use the template in section 3 of this page, verbatim |
| **Weight** | **10% of the project grade** — pass 10% / partial 5% / fail 0% (directives §8.1) |
| **Scored on** | **Whether you did the work.** *Not* on whether your questions turn out to be right |
| **Late** | 10% of the project grade per midnight, **capped at 30%** (directives §10) |
| **Feedback** | Written feedback on every proposal, returned around **Thu Sep 24** |
| **Purpose** | To get you feedback while your direction can still change cheaply |

---

## 2. What must already be true before you write it

Create the GitHub repository **before the proposal**; its link is slot 0. Public or private is your choice — **if private, add the instructor and the TAs as collaborators** (§6.3).

**Remember, no protected attribute may be the thing you predict.** Protected attributes may still be discussed as a *fairness question about a model you built* — that is legitimate and interesting (§3, rule 5).

---

## 3. The template

Use it as it stands. Every slot gets an answer that is specific to *your* dataset.

```
BA305 Project Proposal — Fall 2026
Team name:              Members (full names):

0. TEAM REPOSITORY
   GitHub link (if private, add the instructor and TAs as collaborators):

1. DATASET
   Which pool dataset you were allocated (number and name):

2. PREDICTIVE QUESTION
   The question, in one sentence:
   Which variable you intend to estimate:
   Classification or regression:
   Who would act on the answer, and what would they do differently:

3. DESCRIPTIVE QUESTION
   The question, in one sentence:
   What you expect the structure to tell you:
   Who would act on the answer, and what would they do differently:

4. WHAT YOU ALREADY SEE IN THE DATA
   Two or three sentences on what a first look showed — missing values,
   an imbalanced class, an obviously skewed variable, anything surprising.
   One chart is welcome but not required.

5. RISKS
   What could make this project fail, in your own assessment.

6. WHAT YOU WANT FROM US
   One specific question for the instructor.
```

---

## 4. Slot-by-slot guidance

### Slot 0 — Team repository

The repo is the whole code submission in November, and it is one of the three ways we see who wrote what. Create it now, not in October. Every member will commit their own work from their own account; Colab's *File → Save a copy in GitHub* is the entire workflow. Getting-started links are in §6.3 of the directives.

### Slots 2 and 3 — your two questions

The project needs **two questions: one predictive, one descriptive.**

- **Predictive** — the data estimates one variable from the others. You choose which variable; defending that choice is part of the work.
- **Descriptive** — what is actually *in* the data: which variables move together, what the main axes of variation are, how the cases spread out.

**Two tests your questions must survive (§5.1):**

1. **Could you say, in advance, what result would surprise you?** If every plausible answer would seem reasonable, the question is too shallow to be worth asking.
2. **Could the question be copied word-for-word onto a completely different dataset?** If so it is too generic. A strong question names the specific things being compared and the specific way they might differ.

A question also fails if it can be answered by a single chart or one summary statistic, or if it merely restates a method.

|  |  |
| --- | --- |
| ❌ | *"Can we run PCA on the listings?"* — restates a method, says nothing about what we would learn |
| ❌ | *"What factors affect price?"* — true of any dataset, and answerable with one correlation table |
| ✅ | *"Do listings that advertise square footage command a different rent, at the same bedroom count and neighbourhood, than listings that omit it — and what would that say about how landlords signal quality?"* — names the comparison, names the confounders to hold fixed, and has an outcome that would genuinely surprise you either way |

**"Who would act on the answer, and what would they do differently"** is not a formality. Your answer has to be useful to somebody: someone should be able to do something differently once they know it. That is what rubric item 1 scores in November, and it is the one part of the final rubric the proposal genuinely previews.

### Slot 4 — what you already see in the data

Two or three sentences from a first look: missing values, an imbalanced class, an obviously skewed variable, anything surprising. **This is the slot that shows you checked the dataset beyond the superficial.** A chart is welcome, not required.

### Slot 5 — risks

Your own honest assessment of what could make the project fail. *"We are not sure this is answerable from this data, and here is why"* is a legitimate thing to write here.

### Slot 6 — what you want from us

**One specific question for the instructor** — one a generic team could not have asked. This is the slot where the feedback you get back is worth the most to you, so spend the question well.

### What the proposal does *not* ask for

**You are not committing to methods.** By Sep 17 you will have seen visualization and PCA and nothing else. You may change your methods, and even your questions, at any point up to **Workshop 1 (Fri Oct 16)** — just say so in your Workshop 1 update.

---

## 5. How it is graded

**Three outcomes. Nothing in between** (directives §8.1).

|  |  | What it means |
| --- | --- | --- |
| **Pass** | **10%** | Every slot in the template is answered with something specific to *your* dataset. Slot 4 shows you actually opened the file. Your question in slot 6 is one a generic team could not have asked. **This is the expected outcome** — most teams that take an hour over it land here |
| **Partial** | **5%** | Submitted, but thin: questions in a sentence that would fit any dataset, slot 4 written without opening the data, or a slot left effectively blank |
| **Fail** | **0%** | Not submitted, or with so little content that there is nothing to give feedback on |

A proposal whose questions we tell you to change is still a Pass if the page shows you did the work.

### Where the proposal sits in the project grade

|  | Weight |
| --- | --- |
| **The proposal** | **10%** of the project grade |
| **The final deliverable** — report, slides, presentation, repo, scored on the 100-point rubric in §8.2 | **90%** of the project grade |

The project is **30% of the course grade**.

---

## 6. Late policy (§10)

**10% of the project grade for each midnight that passes after the deadline.**

The proposal is an **early item**, so its deduction is **capped at 30%** — as are team registration and the ranked dataset choice. The deduction stops growing there, but the item is still expected: one never submitted at all takes the full 30% **and** forfeits its feedback.

---

## 7. Writing it — the AI policy applies (§9)

**Generating text with Generative AI is not allowed.** Every word of the proposal, the report and the slides must be written by you.

- **Prohibited:** having a tool write, draft, expand, rewrite, summarise or "polish" any prose — including a paragraph you then edit, and including a bullet list you then turn into sentences.
- **Permitted:** light grammatical correction — spelling, punctuation, agreement, a clumsy clause straightened out. The thinking, the structure, the argument and the wording must be yours.
- **Permitted:** ideation and coding — thinking through approaches, having a concept explained back to you, debugging, help writing code. Code assistance must be **labelled in the code and disclosed**.
- **You are fully responsible for everything you submit.** You may be asked to explain any part of it; inability to do so is handled under the Academic Conduct Code.

---

## 8. Before you submit — checklist

- [ ] One page. PDF. One submission for the whole team, on Blackboard.

- [ ] Team name and **full names** of every member at the top.

- [ ] **Slot 0** — repo link included, and it opens. If private, instructor and TAs added as collaborators.

- [ ] **Slot 1** — the dataset number *and* name, matching the Piazza allocation.

- [ ] **Slot 2** — predictive question in one sentence; the variable you will estimate; classification or regression; who acts on the answer. The target is **not** a protected attribute.

- [ ] **Slot 3** — descriptive question in one sentence; what you expect the structure to tell you; who acts on it.

- [ ] Both questions survive the two tests under *Slots 2 and 3* above — you can say what result would surprise you, and neither question could be pasted onto a different dataset unchanged.

- [ ] **Slot 4** — written from the actual file, naming something concrete you saw in it.

- [ ] **Slot 5** — a real risk, in your own assessment.

- [ ] **Slot 6** — one specific question, not a generic one.

- [ ] Every word written by your team.

---

## Source map

| What | Where it is defined |
| --- | --- |
| Deadline, weight, template, pass/partial/fail scale, late policy, AI policy | `PROJECT_DIRECTIVES.md` §1, §4, §8.1, §9, §10 |
| Dataset pool, allocation rules, protected-attribute rule | `PROJECT_DIRECTIVES.md` §3 · allocation posted on Piazza Fri Sep 11 |
| Question tests, predictive/descriptive definitions | `PROJECT_DIRECTIVES.md` §5.1 |
| Repository requirement and getting-started links | `PROJECT_DIRECTIVES.md` §6.3 |
| Final rubric the proposal previews (item 1, Goals) | `PROJECT_DIRECTIVES.md` §8.2 |
| Project weight (30%), late scale, team registration | The course syllabus — *Group project* and *Term project* |
