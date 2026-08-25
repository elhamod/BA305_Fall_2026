# BA305 — Term Project Directives

**Fall 2026 · Prof. Mohannad Elhamod · 30% of the course grade**

> This document is the single source of truth for the term project. Treat it as both a roadmap and the grading rubric. Where it conflicts with an announcement on Blackboard, Blackboard is correct.

---

## 1. At a glance

| When | What | Graded? |
| --- | --- | --- |
| **Thu Sep 3** (Session 1) | Project introduced in class | — |
| **Thu Sep 10** (Session 3) | **Teams registered on Blackboard**, with your **ranked top three datasets** (§3) | Ungraded — **late penalty applies (§10)** |
| **Fri Sep 11** | **Dataset allocation posted on Piazza** | — |
| **Thu Sep 17** (Session 5) | **Proposal due** (1 page, PDF, one per team) — includes your **repo link** | Ungraded — **late penalty applies (§10)** |
| ~Thu Sep 24 | Written feedback returned on every proposal | — |
| **Fri Oct 16** (Session 14) | **Workshop 1** — progress check on work already underway | — |
| **Mon Oct 19** | **Presentation-slot poll opens on Piazza** (§7) | — |
| **Fri Oct 23, 11:59 PM** | **Poll closes** — no response means you are placed wherever there is room | — |
| **Fri Nov 6** (Session 22) | **Workshop 2** — feedback on your analysis and your argument | — |
| **11:59 PM, night before your slot** | **Slides due** — final version; **cannot be changed after you present** | Graded (§8) |
| **Thu Nov 12 / Tue Nov 17 / Thu Nov 19** | **Presentations** (Sessions 24–26) — 7 min + 8 min Q&A | Graded (§8) |
| **Mon Nov 23, 11:59 PM** | **Written report + code repository due** | Graded (§8) |

There is **no weekly homework** in this course. The project takes its place, and it is expected to progress steadily from mid-September. The workshops are checkpoints on work already in flight — they are not the point at which the work should begin.

> Advice from last year's students, almost unanimously: **start early.** The teams that struggled were the ones that started building in November.

---

## 2. Teams

- **Teams are expected to be four students.** If the class size leaves a group who cannot form a team of four, come and talk to us — a different team size will be agreed for that group.
- You form your own teams and **register on Blackboard by Thu Sep 10, 11:59 PM**. The registration form also asks for your **ranked top three datasets** from the pool in §3, so look through it before you register — not after.
- **Registration is not graded, but it is subject to the project late policy (§10):** a team that registers after the deadline loses **10% of its project grade per day, to a maximum of 30%** — the same rule that applies to the proposal and the report. Register on time; it is the cheapest 30% you will ever protect.
- If you are **not on a registered team** by Sep 10, you will be placed on one. In that case the deduction applies to **your individual project grade**, not to the grade of the team that receives you — a team that registered on time is not penalized for absorbing a latecomer.
- **Every member owns the whole project.** Research, coding, writing, and presenting are shared. You may be asked in Q&A to explain any part of the work, including parts you did not personally write.

---

## 3. Your dataset

**You do not find your own data, and you do not simply take the one you want.** You **rank three datasets** from the pool below, in order of preference, and you are **allocated one**.

Every dataset here has been checked: it is large enough to model, has a genuine mix of numeric and categorical information, contains real missing data, and has enough rows per variable that a careful model will neither memorise the data nor be starved of signal.

**What is NOT given to you — deliberately.** No target variable, no research question, no suggested method, and no description of what is wrong with the file. Working out *what this data actually contains* and *what is worth asking of it* is the first and most important part of the project, and it is scored (rubric items 1 and 3). Two teams on the same dataset should not arrive at the same questions.

### Rules

1. **Rank three datasets, first to third**, on the team registration form due **Thu Sep 10**. The allocation is posted on Piazza the next day, **Fri Sep 11**, and both of your questions come from the dataset you are given.
2. **You may not get your first choice.** Preferences are honoured where possible, but the class as a whole should not spend the presentation block on fourteen versions of the same file. Rank three you would actually be happy with, not one you want and two you do not.
3. **Look before you rank.** Open each folder, read the file, look at the columns, and check that you can imagine a question worth answering. Ten minutes now is worth a week in October.
4. Two teams may be given the same dataset. If that happens you will be asked at the proposal stage to differentiate your questions.
5. **No protected attribute may be the thing you predict.** Race, sex, ethnicity, religion, disability and age are not targets in this course. Where a dataset contains them, they may be discussed as a fairness question *about a model you built* — that is a legitimate and interesting angle — but they are never the variable you set out to estimate.

---

### The pool

Nineteen datasets. Roughly half concern a business decision directly; the rest do not, and that is deliberate — a good analytical question can be asked of a rodent census or a chess archive as readily as of a rent roll. Whichever you are given, **your answer has to be useful to somebody: someone should be able to do something differently once they know it.** That is what rubric item 1 scores, and it is harder on some of these than others.

**Each link goes to the dataset's home, and every one of them documents its own data** — a page or readme listing each column and what it means. Read it before you rank.

**Some of these are more than one file.** Where a dataset comes as several related files, you may use whichever of them you like, and **joining them is welcome** — a question that needs two files joined is often a more interesting question than one that does not.

**1 · San Francisco Bay Area rental listings** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-07-05)

Rental advertisements posted on Craigslist across the Bay Area between 2000 and 2018, scraped and cleaned by economist Kate Pennington for her research on construction and displacement. One row per listing.

**2 · Repair Café repair logs** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2026/2026-04-07)

Repair Cafés are community events where volunteer fixers help people mend broken household items rather than throw them away. One row per item someone brought in, at hundreds of branches across 25 countries.

**3 · Ravelry yarn catalogue** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-10-11)

A snapshot of the yarn catalogue maintained by members of Ravelry, the social network for knitters, crocheters, spinners and weavers. One row per yarn product.

**4 · Billboard Hot 100 tracks with Spotify audio analysis** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2021/2021-09-14)

Every song that has appeared on the Billboard Hot 100 since 1958, matched against Spotify's own acoustic analysis of the recording, alongside the week-by-week chart history.

**5 · BoardGameGeek game catalogue** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-01-25)

Published tabletop games from the internet's largest board-game database, with their design attributes, the counts of how many site members own, want or trade each one, and the community's ratings and rankings.

**6 · UK gender pay gap filings** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-06-28)

Since 2017, UK law has required every employer with 250 or more staff to file gender pay gap statistics each year. This is the public download of those filings.

**7 · Allrecipes recipe archive** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2025/2025-09-16)

Recipes published on Allrecipes.com between 2004 and 2025, with their ingredients, per-serving nutrition, preparation times and community feedback.

**8 · IMDb holiday films** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2023/2023-12-12)

Every movie, TV movie and direct-to-video release in IMDb's catalogue whose title contains a festive keyword, from the late 1920s to 2023, with runtime, genre and audience ratings.

**9 · Flavors of Cacao chocolate bar reviews** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-01-18)

Expert reviews of craft chocolate bars, collected over many years by a critic who buys, tastes and scores bars from around the world. One row per bar.

**10 · Hollywood films with Bechdel Test results** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2021/2021-03-09)

FiveThirtyEight's dataset for its investigation into how Hollywood writes women: Bechdel Test verdicts paired with budgets, box office and IMDb details for films released between 1970 and 2013.

**11 · UK Mapping Museums database** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-11-22)

UK museums surveyed and coded by the Mapping Museums project between 1960 and its close in 2021, with governance, subject matter, size, and statistics describing the surrounding neighbourhood.

**12 · Portal Project desert rodent captures** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2023/2023-05-02)

A field experiment running since 1977 in the Chihuahuan Desert near Portal, Arizona, where fenced study plots control which rodents can enter. One row per animal caught on a census night, plus the plot and species reference tables.

**13 · Lichess online chess games** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-10-01)

Games played on Lichess.org, the free open-source chess server, between 2013 and 2017. One row per game.

**14 · NHL team rosters, 1917–2024** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-01-09)

Every National Hockey League team's roster for every season from 1917–18 through 2023–24, reconstructed from the league's own public API.

**15 · Hotel booking records** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2020/2020-02-11)

Two Portuguese hotels — one a city hotel, one a resort — released their entire booking ledger for 2015 to 2017, anonymised for research. One row per booking.

**16 · New York City elevator registry** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2022/2022-12-06)

Every registered elevator device in New York City, released by the Department of Buildings in response to a 2015 public-records request. One row per device, recording its type, specification, location and inspection record.

**17 · Portuguese bank marketing campaign** — [folder](https://archive.ics.uci.edu/dataset/222/bank+marketing)

A Portuguese retail bank ran repeated telephone marketing campaigns and logged every call. One row per client contact, with the client's details, the call, and the economic conditions of the quarter. *(The download holds several versions of the same campaign — pick one or more and say which. Every column is described on the page under **Additional Variable Information**.)*

**18 · Stack Overflow Developer Survey 2024** — [folder](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-09-03)

The annual survey of working software developers, run by Stack Overflow since 2011: experience, role, employer, working arrangements, tools and pay, one row per respondent.

**19 · US Census income extract** — [folder](https://archive.ics.uci.edu/dataset/2/adult)

Drawn from the 1994 US Census by Ronny Kohavi and Barry Becker, one row per surveyed adult: demographics, employment, and which side of a $50,000 income threshold the person fell on. *(Every column is described on the page under **Additional Variable Information**.)*

---

## 4. The proposal — due Thu Sep 17

**One page, PDF, one per team. Ungraded, but required.** Its only purpose is to get you written feedback while your direction can still change.

By Sep 17 you will have seen visualization and PCA and nothing else. **The proposal does not ask you to commit to methods.** You may change your methods, and even your questions, at any point up to Workshop 1 — just say so in your Workshop 1 update.

Use this template:

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

**Late proposals** are subject to the project late policy (§10).

---

## 5. What the project must contain

These are the **musts** — the floor, not the target. §8 does not score whether you ticked them off; it scores how well you understood the choices behind them and whether you achieved what you set out to do.

### 5.1 Two questions

Formulate **two questions of interest** from your dataset — **one predictive and one descriptive**.

- The **predictive** question asks the data to estimate one variable from the others. You choose which variable; defending that choice is part of the work.
- The **descriptive** question asks what is actually in the data — which variables move together, what the main axes of variation are, how the cases spread out and where they concentrate. The tools are the ones this course teaches for exactly that: **charts and visual analysis** (Sessions 2–3), **PCA** (Session 4), and **t-SNE or UMAP** (Session 5).

Each must be answerable from the data, and each must matter to somebody outside this classroom. Nobody will tell you what these questions are.

**Two tests your questions must survive.**

1. **Could you say, in advance, what result would surprise you?** If every plausible answer would seem reasonable, the question is too shallow to be worth asking.
2. **Could the question be copied word-for-word onto a completely different dataset?** If so it is too generic. A strong question names the specific things being compared and the specific way they might differ.

A question also fails if it can be answered by a single chart or one summary statistic, or if it merely restates a method.

| | |
| --- | --- |
| ❌ | *"Can we run PCA on the listings?"* — restates a method, says nothing about what we would learn. |
| ❌ | *"What factors affect price?"* — true of any dataset, and answerable with one correlation table. |
| ✅ | *"Do listings that advertise square footage command a different rent, at the same bedroom count and neighbourhood, than listings that omit it — and what would that say about how landlords signal quality?"* — names the comparison, names the confounders to hold fixed, and has an outcome that would genuinely surprise you either way. |

### 5.2 Methods — at least two per question

For **each** question, apply and compare **at least two different methods**, chosen to suit the task rather than because they looked impressive.

- **Predictive:** two of k-NN, Naïve Bayes, logistic regression, decision trees, regression trees, neural networks. *"How does a decision tree compare with k-NN here, and which would I deploy?"* is the shape of it.
- **Descriptive:** two of a **structured visual analysis** (a deliberate set of charts that compare groups or track a relationship across a third variable — not one scatter plot), **PCA**, or a **t-SNE / UMAP embedding** — or the same method under two genuinely different choices (a different number of components, a different perplexity, scaled versus unscaled) where you argue for one. *"What do the charts say about how these groups differ, and does PCA agree once all the variables are in play at once?"* is the shape of it. **A pair of methods that are both charts is fine** if the two are genuinely different views of the question.

### 5.3 Data and pipeline, defined concretely

**Data.** State plainly:

- what your **inputs** and **outputs** are;
- the **data type** of each (categorical vs. numerical, and ordinal vs. nominal where it matters);
- what **transformations and cleaning** you performed and why — missing values, one-hot encoding, normalization or standardization, thresholding, outliers, class imbalance.

**Think carefully about which columns you use as features.** For every column, ask what it would let the model learn. Is a customer ID a useful pattern, or is it unique to that one row and therefore worthless for anything you have not already seen? Not every column in a file is information about the case; some are only labels for it. Deciding which is which is your job, and the pool contains columns that will tempt you.

**Feature leakage.** For every input feature, ask: *would this value actually be known at the moment the prediction has to be made?* Features recorded **after** the outcome — or derived from it — must be removed and the removal justified in the report. A model that quietly uses a post-outcome feature looks excellent and is worthless. The test is chronological, not statistical: if you are predicting whether a loan will default, the applicant's income and credit score are known when the loan is approved and are legitimate inputs, while the number of missed payments, the collections flag and the recovery amount are all recorded *after* the outcome you are trying to predict and are not. A feature that is strongly predictive for no reason you can explain is the usual symptom — check its timing before you celebrate it. **If your dataset contains such a feature, naming at least one you dropped for this reason is required.** If after looking properly you are satisfied there is none, say so in the report and say how you checked — that is an acceptable answer, and an unexamined silence is not.

**Split discipline.** Perform a train/test split or cross-validation, and fit every transformation (scaler, PCA, imputer) **on the training data only**. Fitting a scaler on the full dataset before splitting leaks test-set information into training. Inside cross-validation this must happen per fold — that is what `sklearn.pipeline.Pipeline` is for.

**Pipeline diagram.** Show the flow of information from raw input to final output as a diagram, as demonstrated in class. It must make clear what goes in, what the stages are, and what comes out.

### 5.4 Evaluation

**For the predictive question:**

- Use **the right metric for the task**, and say why it is the right one.
- **Accuracy alone is not sufficient.** Address class imbalance and choose a classification threshold deliberately, with an argument for the cutoff you picked.
- **Diagnose the fit.** Is the model overfitting, underfitting, or fitting well? Show the evidence.
- **Tune at least two hyperparameters**, and say how you tuned them (manual sweep, grid search, cross-validated search).
- **Compare your two methods** on the same metric, on the same split, and say which you would deploy and why.

**For the descriptive question**, "evaluation" means showing that what you found is really in the data rather than produced by the way you chose to look at it.

**Start with the charts, and take them seriously.** Two full sessions of this course are about reading and building them, and a descriptive answer carried by well-made figures is a complete answer — not a warm-up for something more impressive. PCA and the embeddings are there for when a chart cannot hold the number of variables you care about, not as a way of looking more advanced.

- **A chart is evidence, and it can be wrong the same way a model can.** In the Session 3 laptop case, a bar chart of store averages made a 2.8% spread look decisive; the same data as a boxplot showed within-store price ranges that swamped the difference entirely. Same data, opposite conclusion, and only one of them was honest. Ask of every figure you rely on: *would a different but equally reasonable chart of this data support a different conclusion?* If it would, show both and say why one is the right reading.
- **Show the spread, not just the middle.** A bar of group means hides exactly what you need in order to know whether a difference matters. If you compare groups, show the variation inside them.
- **Hold the other variables still.** A two-variable comparison that ignores an obvious third variable is the visual version of an unadjusted claim. Use colour, facets or small multiples to hold it fixed — and choose the encoding deliberately: a categorical palette for categories, a sequential one for quantities.
- **Match the chart to the data, and to the claim.** A line asserts that the space between two points means something. A truncated axis asserts that a small difference is a large one. A skewed variable plotted raw lets one extreme value draw the whole picture, where a log scale would show the pattern. Each of these is a claim you are making, not a formatting choice, and you can be asked to defend it.
- **Be as willing to reject a premise as to confirm one.** "We looked, and the pattern people assume is there is not there" is a real finding, and often a better one than the pattern you went looking for.

**Then, where the question genuinely needs more variables than a chart can hold:**

- **Match the method to the data type.** PCA and the distance-based embeddings are defined for **numeric** features. One-hot encoding a categorical column and feeding it straight to PCA is not a neutral convenience — it silently asserts that every pair of categories sits the same distance apart. If your descriptive question is really about categorical data, either restrict to the numeric features and say so, or use a chart that handles categories honestly. Whichever you pick, justify it.
- **Justify how much structure you kept** — how many principal components, and on what evidence. A scree plot and the cumulative explained variance are the arguments; "we took two because it plots nicely" is not one. And say whether you scaled: PCA changes completely on unscaled data.
- **Read t-SNE and UMAP with the caution Session 5 gives them.** In these plots the distance between two blobs, and the size of a blob, are not interpretable. An embedding is a place to look for something, not evidence that it is there.
- **Bring it back to the variables.** Say what a component means in the language of the data, and show the thing you found in a plot of the original variables where you can. A structure that only exists after the transformation, and that you cannot point to in the data itself, is a fragile finding.
- If the structure is weak — the variance is spread thinly across many components, the groups you expected do not separate — **say so**. That is a legitimate and interesting result, and it scores better than a picture squinted at until it agrees with you.

### 5.5 Interpretation

Do not just report numbers.

- Report the **findings and insight** the numbers convey, in plain English that anyone in the room can follow. In your career you will be explaining this to people who do not know what an F1 score is.
- Use **visualizations** where they help you understand the data or communicate the result. **Every figure you show, in the report or on a slide, must have:** axis labels and a legend where applicable; a **one-line caption saying what the reader should conclude from it**; and, if it is complex, a pointer to the part that matters. A figure without a takeaway is decoration.
- Tell the **story of how the model improved** — what you tried, what failed, what you changed, what it bought you. A project that reports only the final number is missing the most interesting part.

---

## 6. Final project deliverables, due at the end of the course

All submitted through Blackboard.

### 6.1 Written report — due Mon Nov 23, 11:59 PM

- **A single PDF.** Times New Roman, 12 pt, 1-inch margins.
- **Maximum 10 pages** for the main body, **including every figure you put in it**, and excluding the cover page and appendix. Be very selective about which figures are load-bearing for your story and which are secondary — the secondary ones belong in the appendix, and a page spent on a chart that carries no argument is a page you did not spend on the argument. The appendix has no page limit: put extended discussion, secondary figures, and sources there.
- One report per team.

**The report must be self-contained.** If a claim needs a figure or a number to be understood, that figure or number belongs in the report or its appendix. **We will not open your notebook to find something the report left out** — anything missing is simply missing, and is marked as such.

**Two sections are required in every report:**

- **Limitations.** What might be wrong, uncertain, or sensitive to a choice you made? What was inconclusive? What would you do with more time or better data, and why? A report with no limitations section reads as a report whose authors did not look for any.
- **Contribution table.** One row per team member, listing the concrete technical tasks that person personally carried out and which methods they ran (*"cleaned the missing-value columns and tested median versus drop"*, *"ran PCA scaled and unscaled and produced the scree-plot comparison"*). Plain English, no jargon, no vagueness. **Writing slides, editing prose, and coordinating the team do not count as technical contribution** — those are expected of everyone and are not what this table records. Each row must also **name the specific files or notebook sections** that person wrote, so the table can be checked against the comments in the code and the repository's commit history (§6.3).

### 6.2 Slides — due 11:59 PM, one day before your signed-up slot

Presentation slots are assigned from a **Piazza poll that closes Fri Oct 23** (§7). Once your slot is posted, your deck is due **11:59 PM the night before it** — so different teams have different slide deadlines.

One deck per team, **submitted to the single `Project slides` assignment on Blackboard**. There is one assignment for all teams, not one per presentation day; **your own deadline is the night before your own slot**, and submission timestamps are checked against it. Submitting early is fine and encouraged; submitting after your slot's midnight is late under §10 no matter what the Blackboard page shows as open.

**Name the file exactly:** `Section_Team##_ProjectTitle.pptx` (or `.pdf`).

**Presentations run from the instructor's computer, using the file you submitted to Blackboard.** You will not connect your own laptop. This is why the deadline is the night before and why the deck is final — the version that runs in the room is the version you handed in.

> **The slides you submit are the slides you present, and they are the slides that are graded. They cannot be changed afterwards.** You may not revise a deck after seeing the questions it drew or after hearing another team's talk. Submit the final version.

Your Nov 23 documentation package must contain this same, unmodified deck. Late slides fall under §10.

### 6.3 Code — due Mon Nov 23, 11:59 PM

**Your team keeps a GitHub repository for the project.** It is where your code lives, and it is one of the three ways we see who wrote what.

- **Create the repo before the proposal** and put its link in the proposal (§4). Public or private is your choice — if private, add the instructor and the TAs as collaborators.
- **Every member commits their own work from their own GitHub account.** One person uploading the whole project at the end defeats the purpose, and a commit history showing a single author invites hard questions in Q&A.
- **You do not need the command line.** Colab has *File → Save a copy in GitHub*, which is the whole workflow: work in Colab, save to the repo under your own account when you finish a piece. Ask on Piazza if you get stuck; do not let a tooling problem eat a week.

**If you have never used GitHub before, start here.** None of this is taught in class — it is a tool, not course content — but you do need it to work, so these four short pages are the whole of what you need. Read them in the first week, not the week the report is due.

| What you need | Where |
| --- | --- |
| What a repository, a commit and a branch actually are — 30 minutes, no coding, no command line | [GitHub Docs — Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) |
| The simplest workflow, if you work only in Colab | Colab: *File → Save a copy in GitHub* — nothing else to install |
| Running and editing `.ipynb` notebooks in VS Code on your own machine | [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) |
| Cloning, committing, pulling and pushing from VS Code — all buttons, no terminal | [Quickstart: use source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/intro-to-git) and [Work with GitHub in VS Code](https://code.visualstudio.com/docs/sourcecontrol/github) |

Either route is fine and you can mix them — Colab for running things, VS Code when you want to edit locally. What matters is only that **your own commits appear under your own account**.
- The final notebook must **run top to bottom with no errors** from a fresh Colab runtime. Restart the runtime, Run All, and confirm before you submit.
- Organized and commented well enough that a classmate could follow it.
- **Submit the link to your repository — that is the whole code submission.** Do not upload notebooks or data files separately; the repository is what we open and what we grade.
- **The code is frozen at the deadline.** Nothing in the repository may be changed after **Mon Nov 23, 11:59 PM** — commit timestamps are visible to us, and a commit after the deadline is a late submission under §10 regardless of what it changed.

#### Attribution — three layers, and they must agree

1. **A comment at the top of every section you wrote**, naming you:
   `# --- Priya: preprocessing, missing-value handling, imputation choice ---`
2. **Your own commits** in the team repository.
3. **The contribution table** in the report (§6.1).

> **Putting your name on a section is a claim you will be asked to defend.** If you are asked in Q&A about a block of code with your name on it and cannot explain what it does and why you did it that way, that is worse than not having claimed it — it is a statement about the work that is not true. Claim what you did; do not claim what you did not.

> The repo does not relax the self-contained rule in §6.1. The report is graded on what the report contains; the repo is how contribution and reproducibility are checked.

> **Resubmission:** if you resubmit any Blackboard item, you must re-upload **all** of that item's files — earlier submissions are discarded and only the final one is graded. This applies to the report and the slides. The code is not resubmitted at all: we take whatever the repository holds at the deadline (§6.3).

---

## 7. Presentation and Q&A

**Format: 7 minutes presenting + 8 minutes Q&A, 15 minutes per team.**

**The clock is enforced and the cost is stated in advance.** Every minute you run over 7:00 costs **10% of your presentation score**. At **8:00 you are stopped mid-sentence**, and whatever you had not yet said does not get said. If your team is not ready when called, you go to the end of the session and lose the minutes you wasted from your own 7. Rehearse with a timer, out loud, more than once.

**Every member speaks, and each person presents their own work** — not a section someone else did. A team where one person narrates everything has told us something about how the work was divided.

**Slots are assigned from a ranked-preference poll on Piazza, not first-come.** The three presentation days are not equivalent — a later day gives you more working time, and your slides lock at your slot — so a race to click would hand a real advantage to whoever refreshes fastest. Instead:

- **Mon Oct 19** — the poll goes up on Piazza. It lists the possible orderings of the presentation days; your team picks the one it prefers. One response per student; your team's answer is the majority of its members.
- **Fri Oct 23, 11:59 PM** — the poll closes. **A team that does not respond is treated as indifferent** and is placed wherever there is room.
- Shortly after, the assignment is posted on Piazza. It maximizes the number of teams getting their first choice, and the allocation is run by a published script rather than by hand.

Slots per session are below. **The format is identical in both sections** — every team in this course gets the same 7 + 8 minutes, so that every team is graded against the same standard.

- **Section A (10 teams):** 4 slots in Session 24, 3 in Session 25, 3 in Session 26.
- **Section B (4 teams):** 2 slots in Session 24 and 2 in Session 25. Session 26 is not a presentation session in Section B — it is an **open working session**: bring a data problem you are curious about and we will work on it together in class.

Whichever slot you take, **your slides are due 11:59 PM the night before it** (§6.2).

> **Extenuating circumstances.** If a religious observance, a documented accommodation, a medical situation, or an obligation you genuinely cannot move affects which day you can present, **contact the instructor on Piazza before the poll closes on Fri Oct 23** — not after slots are assigned. Conflicts raised before the deadline are accommodated wherever possible. Once slots are assigned they are final, so raise it early even if you are not certain yet.


### What goes in the 7 minutes

Seven minutes is not enough to walk through your project. It is not supposed to be. **Your report carries the detail; the talk carries the argument.** Budget roughly:

| | |
| --- | --- |
| **The problem** — what you asked and why anyone should care | ~1.5 min |
| **Your approach** — the dataset, and the shape of what you did | ~1.5 min |
| **What you found** — the headline result for each question, and how confident you are in it | ~2.5 min |
| **What it means** — the decision someone could make differently | ~1.5 min |

**Deliberately minimize or leave out** of the talk: your preprocessing steps one by one, every hyperparameter you swept, every chart you made, and the code. Those belong in the report, and we will ask about them in Q&A. A team that spends two minutes on one-hot encoding has spent two minutes not making its argument.

**Explain the problem before the solution.** A talk that opens with model architecture has lost the room.

**No jargon, no name-dropping, no fancy words you cannot unpack.**

- A technical term may be used only if you **define it clearly the first time** it appears.
- **Naming a method without saying what it does and why you chose it counts against you.** "We used a random forest" is not an explanation.
- A word you cannot explain plainly when asked will cost you more than the simpler word would have. If you cannot explain it simply, you do not understand it well enough yet.

### What Q&A is for

**You are expected to defend your work and to answer questions about its details.** This is the part of the assessment that establishes the work is yours. Questions may be directed at **any member of the team**, about **any part of the project** — including parts you did not personally write. "That was someone else's section" is not an answer.

Expect to be asked things like:

- Why did you choose that method over the alternative?
- Why is that the right metric for this question?
- How do you know the model isn't overfitting?
- What happens to your conclusion if that assumption is wrong?
- Which feature did you drop for leakage, and how did you know to drop it?
- You reported this number — what would you actually tell a manager to do?

**What scores well:** a direct answer with the reasoning behind it. *"We chose that, and here's why"* is a good answer. So is *"we tried that, it didn't work, and here's what we think went wrong."* So is **"I don't know — here's how we'd find out"**, which scores better than a confident guess and much better than a bluff. We are testing whether you understand your own project, not whether you can be caught out.

**What scores poorly:** an answer that repeats a slide instead of addressing the question; a technical term used without being able to unpack it; any claim you cannot trace back to something in your code; and **"I don't know" with nothing behind it** — no idea of where you would look, what you would try, or why the answer is not already in front of you. The good version of not knowing comes with a next step; the poor version is a full stop.

### How Q&A runs

The **first question comes from your classmates**, not from the instructor. The instructor asks after that.

**If you are in the audience, you are part of this session.** Asking a presenting team a substantive question is exactly the kind of contribution the participation policy asks for, and the presentation block is three sessions in which every team should be doing it. The other half of that expectation is the attention rule in the syllabus: follow what is being presented and discussed. If you are asked something and it is clear you were not following, it costs you **10% of your participation grade** (§ *Class participation* in the syllabus).

Q&A is not a cross-examination and it is not about typos. It is a professional conversation about a piece of work, which is what these conversations look like after you graduate.

## 8. Grading rubric — 100 points

This rubric scores two things: **whether you understood what you were doing**, and **whether you achieved the goals you set**.

It does not score whether you produced a checklist of artifacts. The requirements in §5 are the **floor, not the target** — doing all of them mechanically, with no evidence of understanding behind the choices, is an *Acceptable* project, not a good one.

### How each item is scored

Every item uses the same six levels, and the levels describe **understanding**, not effort or volume. Note the gap at the bottom: a genuine attempt that misses the point still earns 70% of the item, but **an item you simply did not do is a zero**. There is no credit for absence.

| Level | % of item | What it means |
| --- | --- | --- |
| **Excellent** | 100% | Correct, and justified with reasoning that shows why the alternatives were worse. The understanding is visible without anyone having to ask for it. |
| **Good** | 92% | Correct, and justified when asked. Minor gaps. |
| **Acceptable** | 87% | Defensible, but the reasoning is thin, generic, or borrowed. The work was done; the thinking is shallow. |
| **Weak** | 80% | Present, but the reasoning is missing, wrong, or contradicts what the code actually does. |
| **Minimal** | 70% | Attempted, but in a way that shows the idea was not understood. |
| **None** | 0% | Not attempted at all. Nothing to grade. |

### The items

| # | Item | Pts | The question we are actually asking |
| --- | --- | --- | --- |
| 1 | **Goals — are they real, and are they yours?** | 10 | Are your two questions specific, answerable from this data, and worth answering? Can you say who would act on the answer and what they would do differently? Everyone starts from the same pool, so the question **is** the differentiator: a question lifted off the obvious column scores below one that took thought. |
| 2 | **Method choices — do you know why you made them?** | 15 | Are the methods suited to the questions, and can you say why *these* rather than the alternatives you rejected? Naming a method is not the same as choosing one. This item is about the **choice**; whether you then ran it correctly is item 3. |
| 3 | **Validity, correctness and technical soundness — is the number you are reporting the number you think it is?** | 20 | Item 2 asks whether you picked a sensible method. **This item asks whether you then executed it correctly.** A well-chosen method run wrongly produces a number that means something other than what you claim, and that is what is scored here: leakage found and removed; every transformation fit on training data only, per fold; a metric that measures what the question asks about; class imbalance and the decision threshold handled deliberately rather than by default; overfitting or underfitting diagnosed **with evidence** rather than asserted; and the code doing what the report says it does. This is the heaviest item, because a result that cannot be believed has achieved nothing. |
| 4 | **Achievement — did you answer your questions?** | 15 | Did you reach an answer for each question, and do you know how good that answer is? **A model that performed poorly is not a failed project.** Honestly establishing that a question *cannot* be answered well from this data — with the evidence, a diagnosis, and what it would take to do better — earns full marks here. Quietly swapping in an easier question, or reporting only the run that worked, earns none. |
| 5 | **Interpretation and communication** | 20 | Do the report and the talk explain the *why*, not just the *what*, to someone who does not know what an F1 score is? Did you prioritize the argument over the detail in the 7 minutes you had? Do the visualizations carry the finding honestly? |
| 6 | **Defense and ownership** | 15 | In Q&A: can **any** member explain **any** part of the work? Honest uncertainty — *"we don't know, and here's how we'd find out"* — scores above a confident guess. A bluff scores below silence. |
| 7 | **Reproducibility** | 5 | Does the notebook run top to bottom from a fresh runtime, and can a classmate follow it? |

**Item 7 carries more weight than its 5 points suggest.** If your code does not run, your results **cannot be verified**, and item 3 is capped at *Minimal* on top of whatever item 7 itself loses. Restart your runtime and Run All before you submit.

**There is no bonus.** Work beyond the course content is welcome, and it shows up where it belongs — in items 2, 4 and 5 — but it never compensates for a project that is not sound. Complexity is not a credential.

---

## 9. Generative AI

The full policy is in the syllabus. For this project specifically:

**Generating text with Generative AI is not allowed.** Every word of your report and your slides must be written by you.

- **Prohibited: having a Generative AI tool write, draft, expand, rewrite, summarise or "polish" any prose** for the report or the slides — including a paragraph you then edit, and including a bullet list you then turn into sentences. If the sentence started as the model's, it does not belong in your report.
- **Permitted: light grammatical correction** — spelling, punctuation, agreement, a clumsy clause straightened out. The kind of thing a spell-checker does. The thinking, the structure, the argument and the wording must be yours.
- **Permitted: ideation and coding.** You may use Generative AI to think through approaches, to explain a concept back to you, to debug, and to help write code.
- **If you use Generative AI to assist with code, you must explicitly label every such block** and disclose it in the required appendix — tool and version, how it was used, and links or screenshots of the exchange.
- **You are fully responsible for everything you submit.** AI-generated errors and hallucinations are your errors.
- The instructor may ask you to explain any part of your work. **Inability to explain your own submission in a way that demonstrates understanding and ownership is treated as evidence that the work is not yours**, and is handled under the Academic Conduct Code. This applies to the writing as much as to the code: if you cannot account for how a passage of your own report came to be phrased the way it is, that is the question you will be asked.

Any violation of the AI policy is treated as a serious honor code violation.

---

## 10. Late policy

**10% of the project grade for each midnight that passes after the deadline**, applied to every dated project item — team registration, the ranked dataset choice, the proposal, the slides, and the report — and **capped at a 30% deduction** in every case.

> The deduction stops growing at 30%. A deliverable is still expected after that: one never submitted at all takes the full 30% *and* forfeits its feedback and the points for its content.

Each item's deduction is applied once, to your project grade. For the slides, "the deadline" means **11:59 PM the night before your own slot**, not the night before the first presentation session. For the code, a commit pushed to your repository after **Mon Nov 23, 11:59 PM** counts as a late submission (§6.3).

---

## 11. Where to ask

**Piazza is the only contact channel for this course.** Post project questions there so the whole class benefits; mark it private if it concerns your team's specific data. Office hours are the right place for anything that needs a screen share.
