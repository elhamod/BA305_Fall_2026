# BA305 — Term Project Directives

**Fall 2026 · Prof. Mohannad Elhamod · 30% of the course grade**

> This document is the single source of truth for the term project. Treat it as both a roadmap and the grading rubric. Where it conflicts with an announcement on Blackboard, Blackboard is correct.

---

## 1. At a glance

| When | What | Graded? |
| --- | --- | --- |
| **Thu Sep 3** (Session 1) | Project introduced in class | — |
| **Thu Sep 10** (Session 3) | **Teams registered on Blackboard** | Ungraded — **late penalty applies (§10)** |
| **Thu Sep 17** (Session 5) | **Proposal due** (1 page, PDF, one per team) — includes your **repo link** | Ungraded — **late penalty applies (§10)** |
| ~Thu Sep 24 | Written feedback returned on every proposal | — |
| **Fri Oct 16** (Session 14) | **Workshop 1** — progress check on work already underway | — |
| **Fri Nov 6** (Session 22) | **Workshop 2** — feedback on your analysis and your argument | — |
| **Thu Nov 12 / Tue Nov 17 / Thu Nov 19** | **Presentations** (Sessions 24–26) — 7 min + 8 min Q&A | Graded (§8) |
| **Mon Oct 19** | **Presentation-slot poll opens on Piazza** (§7) | — |
| **Fri Oct 23, 11:59 PM** | **Poll closes** — no response means you are placed wherever there is room | — |
| **11:59 PM, night before your slot** | **Slides due** — final version; **cannot be changed after you present** | Graded (§8) |
| **Mon Nov 23, 11:59 PM** | **Written report + notebook due** | Graded (§8) |

There is **no weekly homework** in this course. The project takes its place, and it is expected to progress steadily from mid-September. The workshops are checkpoints on work already in flight — they are not the point at which the work should begin.

> Advice from last year's students, almost unanimously: **start early.** The teams that struggled were the ones that started building in November.

---

## 2. Teams

- **Teams are expected to be four students.** If the class size leaves a group who cannot form a team of four, come and talk to us — a different team size will be agreed for that group.
- You form your own teams and **register on Blackboard by Thu Sep 10, 11:59 PM**.
- **Registration is not graded, but it is subject to the project late policy (§10):** a team that registers after the deadline loses **10% of its project grade per day, to a maximum of 30%** — the same rule that applies to the proposal and the report. Register on time; it takes two minutes and it is the cheapest 30% you will ever protect.
- If you are **not on a registered team** by Sep 10, you will be placed on one. In that case the deduction applies to **your individual project grade**, not to the grade of the team that receives you — a team that registered on time is not penalized for absorbing a latecomer.
- **Every member owns the whole project.** Research, coding, writing, and presenting are shared. You may be asked in Q&A to explain any part of the work, including parts you did not personally write.

---

## 3. Your dataset

**You do not find your own data. You choose one dataset from the pool below.**

Every dataset here has been checked: it is large enough to model, has a genuine mix of numeric and categorical information, contains real missing data, and has enough rows per variable that a careful model will neither memorise the data nor be starved of signal. The known traps are noted so you spend your time on analysis rather than on discovering that a column means something other than it appears.

**What is NOT given to you — deliberately.** No target variable, no research question, no suggested method. Working out *what is worth asking of this data* is the first and most important part of the project, and it is scored (rubric item 1). Two teams on the same dataset should not arrive at the same questions.

### Rules

1. **Pick one dataset.** Both of your questions come from it. Register your choice in the proposal (§4).
2. Two teams may choose the same dataset. If that happens you will be asked at the proposal stage to differentiate your questions.
3. **Read the linked description before you commit.** Open the file, look at the columns, and check that you can imagine a question worth answering.
4. If a dataset ships companion files in the same folder, you may join them — say so in the proposal.

---

### The pool

Nineteen datasets. Roughly half concern a business decision directly; the rest do not, and that is deliberate — a good analytical question can be asked of a rodent census or a chess archive as readily as of a rent roll. Whichever you pick, **you must be able to name someone who would act differently once they knew your answer.** That is what rubric item 1 scores, and it is harder on some of these than others.


**1 · San Francisco Bay Area rental listings** — [`rent.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-07-05/rent.csv) · 200,796 rows × 17 columns

Between 2000 and 2018, Bay Area landlords posted hundreds of thousands of rental advertisements on Craigslist. Economist Kate Pennington scraped and cleaned them for her research on construction, gentrification and displacement, and this file holds about 200,000 of those posts. Each row is a single listing: the neighbourhood, city and county, the monthly rent asked in dollars, the number of bedrooms and bathrooms, square footage, whether the ad is for a room in a shared apartment, sometimes a street address or map coordinates, and the poster's own headline and free-text description. Listings span the dot-com era, the housing crash and the tech boom.
> ⚠ Dropping every row with a missing value leaves under 1% of the data — several columns are 90%+ empty while the core fields are nearly complete. Decide which columns to discard rather than which rows.

**2 · Repair Café repair logs** — [`repairs.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2026/2026-04-07/repairs.csv) · 178,749 rows × 11 columns

Repair Cafés are community events where volunteer fixers help people mend broken household items rather than throw them away. Since 2015 the Repair Monitor project has logged what comes through the door, and this file records about 179,000 repair visits at 447 café branches in 25 countries, led by the Netherlands, Britain, France, Canada and Australia. Each row is one item someone brought in: the date, the branch and country, what the object was (vacuum cleaner, toaster, laptop, lamp), its product category and brand, a volunteer's estimate of when it was made, how the attempt ended, and a 1-to-10 rating of how easy it was to work on.
> ⚠ Brand has ~8,600 levels and product type ~1,950 — these need grouping before encoding. Production year is missing for about two thirds of visits.

**3 · Ravelry yarn catalogue** — [`yarn.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-10-11/yarn.csv) · 100,000 rows × 24 columns

Ravelry is a social network for knitters, crocheters, spinners and weavers, whose members maintain a shared catalogue of the yarns they use. This file is a snapshot of 100,000 yarn products pulled from Ravelry's API, one row per yarn. It records the product name and company, the weight category (lace, fingering, sport, DK, worsted, aran) with ply and wraps per inch, grams per skein and yardage, the stitch gauge it knits to, whether it is machine washable, a member-written texture description such as "cable plied", the average rating out of five, the number of ratings behind it, and whether it is still in production.
> ⚠ No row is complete — some columns are 96–100% empty. Drop near-empty columns rather than incomplete rows. Company has ~11,000 levels.

**4 · Billboard Hot 100 tracks with Spotify audio analysis** — [`audio_features.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2021/2021-09-14/audio_features.csv) · 29,503 rows × 22 columns

Sean Miller assembled every song that has appeared on the Billboard Hot 100 since 1958, then looked each one up on Spotify. This file is the Spotify half of that project: about 29,500 tracks, one row per song-and-performer pairing. Alongside the title, performer, album, genre tags and an explicit-content flag, each row carries Spotify's own acoustic analysis of the recording — danceability, energy, key and mode, loudness, speechiness, acousticness, instrumentalness, liveness, valence, tempo and time signature, most scaled between zero and one — plus duration in milliseconds and a popularity score.
> ⚠ About one song in six failed to match on Spotify, so its whole block of audio measures is blank together. Genre is a stringified list that must be parsed. A companion `billboard.csv` in the same folder holds the week-by-week chart history.

**5 · BoardGameGeek game catalogue** — [`details.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-01-25/details.csv) · 21,631 rows × 23 columns

BoardGameGeek is the internet's largest catalogue of tabletop games. Each of the 21,631 rows is one published game and records the year it came out, the minimum and maximum number of players, minimum age, advertised and actual playing times, and a written description, along with bracketed lists of the game's categories, mechanics, families, designers, artists and publishers. Four community-collection counts show how many site members own the game, have it up for trade, want it, or have wishlisted it.
> ⚠ Category, mechanic, designer, artist and publisher are Python-style bracketed multi-value lists that need parsing. A companion `ratings.csv` shares the same game `id` and holds the community ratings and rankings.

**6 · UK gender pay gap filings** — [`paygap.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-06-28/paygap.csv) · 48,711 rows × 27 columns

Since 2017, UK law has required every employer with 250 or more staff to file gender pay gap statistics with the government each year. This is the public download of those filings: roughly 49,000 submissions from about 12,700 employers spanning reporting years 2018 to 2023. Each row names the employer with its address, postcode, Companies House number and SIC industry codes, an employer size band, the mean and median gap between men's and women's hourly pay and bonuses, the share of each sex receiving a bonus, the male and female share of staff in each pay quartile, and the submission date.
> ⚠ The same employer files in up to six different years, so rows are not independent observations. The paired male/female quartile columns sum to 100 and are perfectly redundant with each other. Figures are self-reported.

**7 · Allrecipes recipe archive** — [`all_recipes.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2025/2025-09-16/all_recipes.csv) · 14,426 rows × 16 columns

Allrecipes.com is one of the largest home-cooking sites on the web, and this collection holds 14,426 of its recipes published between 2004 and 2025. Each row is a single recipe with its title, web link, the community member who posted it, the publication date, and the full ingredient list exactly as written. Alongside these are per-serving nutrition figures for calories, fat, carbohydrates and protein, the number of servings, preparation, cooking and total times in minutes, and community feedback in the form of a star rating, a count of ratings and a count of written reviews.
> ⚠ **The rating-count and review-count columns are corrupted** — a scraping error truncated them below 1,000, so no recipe shows more than 997 ratings and the most popular recipes carry wrong numbers. Ingredients is unstructured free text.

**8 · IMDb holiday films** — [`holiday_movies.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2023/2023-12-12/holiday_movies.csv) · 2,265 rows × 14 columns

IMDb publishes bulk downloads of its title catalogue, and this file keeps every movie, TV movie and direct-to-video release whose title contains a festive keyword — Christmas, Xmas, holiday, Hanukkah or Kwanzaa. The result is 2,265 titles stretching from the late 1920s to 2023, from studio classics to obscure made-for-television films. Each row gives the IMDb identifier, the promotional and original-language titles, release year, runtime in minutes, up to three comma-separated genres, the weighted average of user star ratings, the number of votes cast, and flags showing which holiday keyword the title matched.
> ⚠ Genres packs up to three values into one cell and must be split. Runtime is missing for 189 titles. The rows are a keyword filter on IMDb, not a random sample.

**9 · Flavors of Cacao chocolate bar reviews** — [`chocolate.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-01-18/chocolate.csv) · 2,530 rows × 10 columns

These are expert reviews of craft chocolate bars collected by Flavors of Cacao, a long-running public database built by a critic who buys, tastes and scores bars from around the world. Each of the 2,530 rows is one bar. It records the manufacturer and the region the company is based in, the year of the review, the country the cocoa beans came from, the specific bean origin or bar name, the cocoa percentage, a score, a shorthand ingredient list (beans, sugar, cocoa butter, vanilla, lecithin, salt) and a few words describing the bar's most memorable characteristics.
> ⚠ Cocoa percent arrives as text like `"76%"`. The ingredient list is a coded string such as `"3- B,S,C"`. Manufacturer has 580 levels.

**10 · Hollywood films with Bechdel Test results** — [`movies.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2021/2021-03-09/movies.csv) · 1,794 rows × 34 columns

FiveThirtyEight built this dataset for its investigation into how Hollywood writes women, pairing Bechdel Test verdicts from BechdelTest.com with money and IMDb details for 1,794 films released between 1970 and 2013. The Bechdel columns record whether a film has at least two named women who talk to each other about something other than a man, and exactly where a film fell short. Alongside them sit production budgets and domestic and international grosses, given both in release-year dollars and adjusted to 2013, plus IMDb ratings and vote counts, Metascores, running time, genre, language, country of production, and the director, writer and cast.
> ⚠ The file is a join of two sources, so about 200 films have every IMDb-derived field blank. Money appears twice — release-year and 2013-adjusted — as near-duplicate pairs. Three columns encode the same Bechdel judgement in different forms.

**11 · UK Mapping Museums database** — [`museums.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2022/2022-11-22/museums.csv) · 4,191 rows × 35 columns

The Mapping Museums project gathered, cleaned and coded information on more than 4,000 UK museums — almost double the coverage of any earlier survey — spanning 1960 up to the project's close in 2021. Each row is one museum. It gives the name, address, postcode and map coordinates, the years the museum opened and, where relevant, closed, who governs it (a local authority, the National Trust, a private owner, a not-for-profit), its subject matter from farming to boats and ships, a size band, its official accreditation status, and deprivation and geodemographic statistics describing the surrounding neighbourhood.
> ⚠ Opening and closing years are **text ranges** like `"2012:2012"`, with `"9999:9999"` meaning "still open". About 1,200 of the size values are random-forest predictions rather than recorded facts, flagged in a provenance column.

**12 · Portal Project desert rodent captures** — [`surveys.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2023/2023-05-02/surveys.csv) · 28,364 rows × 22 columns

Since 1977, ecologists have run a long-term field experiment in the Chihuahuan Desert near Portal, Arizona, where fenced study plots control which rodents can enter and which are kept out. On regular census nights researchers trap animals at numbered stakes and record the date, the plot and its experimental treatment, the species and sex of each animal caught, its body measurements and reproductive condition, and the ear-tag number identifying it. This file holds roughly 28,000 individual captures collected between 1978 and 2022 — kangaroo rats, pocket mice and their neighbours — from one of the longest-running ecological monitoring efforts in the United States.
> ⚠ Six reproductive-condition columns are 75–99% empty and must be dropped. Species is a two-letter code whose meaning lives in a companion `species.csv`. The plot number fixes the plot's treatment exactly, so pairing those two columns is circular. Animals are re-caught: the same individual can appear up to 38 times, so a naive random split puts the same animal on both sides of it.

**13 · Lichess online chess games** — [`chess.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2024/2024-10-01/chess.csv) · 20,058 rows × 16 columns

Lichess.org is a free, open-source chess server where members play millions of games a day. This file, assembled from a sample of Lichess accounts, records just over 20,000 games played between 2013 and 2017. Each row is a single game and carries the clock setting, whether the game counted toward players' official ratings, the anonymised usernames and Elo ratings of the two opponents, how many turns were played, the manner in which the game finished, the side credited with the win, the complete move list in standard algebraic notation, and the opening played, identified by both its ECO code and its name.
> ⚠ The `moves` column contains the whole finished game, so it gives away almost everything else in the row — including, through the parity of the turn count, the winner of every game that ended in mate. The two timestamps are epoch-millisecond values rounded so coarsely that 42.6% of games appear to last zero time. `opening_name` has 1,477 levels.

**14 · NHL team rosters, 1917–2024** — [`nhl_rosters.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2024/2024-01-09/nhl_rosters.csv) · 54,883 rows × 18 columns

This file reconstructs the roster of every National Hockey League team for every season from 1917–18 through 2023–24, pulled from the league's own public API. Its rows are player-seasons: one line for each of 8,472 men in each year he appeared on a roster. A line carries the three-letter team code, the season, the sweater number he wore, his position code and grouping, whether he shoots or catches left or right, his height and weight at the start of that season in both imperial and metric units, and his birth date, city, country and province or state.
> ⚠ Height and weight each appear **twice**, in imperial and metric — the pairs are the same variable and one of each must go. The detailed position code and the broad position grouping determine one another exactly. The same player recurs for up to 28 seasons with identical physical measurements, so consider reducing to one row per player.

**15 · Hotel booking records** — [`hotels.csv`](https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-02-11/hotels.csv) · 119,390 rows × 32 columns

Two Portuguese hotels — one a city hotel, one a resort — released their entire booking ledger for 2015 to 2017, anonymised for research by Antonio, Almeida and Nunes. Each row is one booking: when it was made and how far in advance, the arrival date, how many weekend and weekday nights were requested, the number of adults, children and babies, the guest's country, the market segment and distribution channel that produced the booking, whether the guest had stayed before, previous cancellations, the room type reserved and the one actually assigned, deposit terms, the average daily rate agreed, car-parking spaces and special requests.
> ⚠ **Two columns record what eventually became of the booking and were filled in after it was resolved.** Ask of every column whether its value would have existed at the moment a judgement would need to be made. Missingness runs at four very different scales, from 4 blanks in one column to 94% in another — that last one forces a real impute-or-drop decision. The daily rate contains zeros and at least one extreme outlier.

**16 · Telecom customer accounts** — [`Telco-Customer-Churn.csv`](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv) · 7,043 rows × 21 columns

A sample telecommunications customer file published by IBM for analytics teaching, describing 7,043 residential subscribers of a fictional but realistically constructed phone and internet provider. Each row is one account and records the customer's basic profile, whether they have a partner or dependants, how many months they have been a subscriber, which services they buy — phone line, multiple lines, internet type, online security, backup, device protection, technical support, streaming television and film — their contract length, whether they use paperless billing, their payment method, their monthly charge, their total charges to date, and whether the account is still active.
> ⚠ Total charges is stored as **text** and contains 11 blank strings, so a missing-value check reports **zero missing** until the column is converted. The customer identifier must be dropped. Total charges is also very close to months-of-tenure multiplied by the monthly charge — think about whether both belong in a model.

**17 · Portuguese bank marketing campaign** — [`bank-full.csv`](https://raw.githubusercontent.com/selva86/datasets/master/bank-full.csv) · 41,188 rows × 21 columns *(semicolon-separated: `pd.read_csv(url, sep=";")`)*

A Portuguese retail bank ran repeated telephone marketing campaigns and logged every call. This file, donated to the UCI repository by Moro, Cortez and Rita, holds 41,188 contacts. Each row describes one client contact: the client's age, job type, marital status, education, whether they carry credit in default, a housing loan or a personal loan, the contact channel and the month and weekday of the call, how long the call lasted, how many times this client was contacted in this campaign and in previous ones, how long since the last contact and how that earlier campaign ended, plus five macroeconomic indicators for the quarter — employment variation, consumer price and confidence indices, the Euribor rate and the number employed.
> ⚠ A missing-value check reports **zero missing**, but six columns encode absence as the literal string `"unknown"` — over 8,000 rows in one of them. The days-since-last-contact column uses **999 to mean "never previously contacted"**, which will wreck any scaled model left as-is. One column could only have been known once the call had already finished.

**18 · IBM HR employee records** — [`emp_attrition.csv`](https://raw.githubusercontent.com/IBM/employee-attrition-aif360/master/data/emp_attrition.csv) · 1,470 rows × 35 columns

A synthetic but carefully constructed human-resources file created by IBM data scientists and now widely used for teaching workforce analytics. Each of the 1,470 rows is one employee, described by age, business travel frequency, department, distance from home, education level and field, job role and job level, monthly income and rate, hourly and daily rates, percentage salary hike, stock option level, total working years, years at the company, years in the current role, years since last promotion, years with the current manager, number of previous employers, overtime status, training attended last year, performance rating, and self-reported scores for job satisfaction, environment satisfaction, relationship satisfaction, job involvement and work–life balance.
> ⚠ The smallest dataset in the pool at 1,470 rows against 35 columns, so this is the one where an over-complicated model will memorise rather than learn. Job role determines department exactly. Several columns are constant for every employee and carry no information at all — find them.

**19 · US Census income extract** — [`adult-all.csv`](https://raw.githubusercontent.com/jbrownlee/Datasets/master/adult-all.csv) · 48,842 rows × 15 columns

Drawn from the 1994 US Census by Ronny Kohavi and Barry Becker, this is one of the most-studied tabular datasets in machine learning. Each row is one surveyed adult and records age, class of worker, a census sampling weight, education level and years of schooling, marital status, occupation, household relationship, race, sex, capital gains and losses, usual hours worked per week, country of birth, and which side of a $50,000 annual income threshold the person fell on.
> ⚠ **The file has no header row.** Supply the column names yourself, or the first record is silently swallowed as headers:
> ```python
> cols = ["age","workclass","fnlwgt","education","education_num","marital_status","occupation",
>         "relationship","race","sex","capital_gain","capital_loss","hours_per_week","native_country","income"]
> df = pd.read_csv(url, header=None, names=cols)
> ```
> Missing values are the string `"?"`, not blanks. **`race` and `sex` are present in this file. Neither may be used as something to estimate** (§3). They may be discussed as a fairness question about the model you build — that is a legitimate and interesting angle.

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
   Which pool dataset (number and name):
   Why this one interested your team (2 sentences):
   Any companion file in the same folder you intend to join:

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
- The **descriptive** question asks what structure is in the data — which cases group together, which variables move together, what the main axes of variation are. PCA and clustering (Sessions 4–5) are the tools.

Each must be answerable from the data, and each must matter to somebody outside this classroom. Nobody will tell you what these questions are.

**Two tests your questions must survive.**

1. **Could you say, in advance, what result would surprise you?** If every plausible answer would seem reasonable, the question is too shallow to be worth asking.
2. **Could the question be copied word-for-word onto a completely different dataset?** If so it is too generic. A strong question names the specific things being compared and the specific way they might differ.

A question also fails if it can be answered by a single chart or one summary statistic, or if it merely restates a method.

| | |
| --- | --- |
| ❌ | *"Can we cluster the listings?"* — restates a method, says nothing about what we would learn. |
| ❌ | *"What factors affect price?"* — true of any dataset, and answerable with one correlation table. |
| ✅ | *"Do listings that advertise square footage command a different rent, at the same bedroom count and neighbourhood, than listings that omit it — and what would that say about how landlords signal quality?"* — names the comparison, names the confounders to hold fixed, and has an outcome that would genuinely surprise you either way. |

### 5.2 Methods — at least two per question

For **each** question, apply and compare **at least two different methods**, chosen to suit the task rather than because they looked impressive.

- **Predictive:** two of k-NN, Naïve Bayes, logistic regression, decision trees, regression trees, neural networks. *"How does a decision tree compare with k-NN here, and which would I deploy?"* is the shape of it.
- **Descriptive:** two of PCA, t-SNE/UMAP, k-means or hierarchical clustering — or the same method under two genuinely different choices (a different number of components or clusters, scaled versus unscaled) where you argue for one.

### 5.3 Data and pipeline, defined concretely

**Data.** State plainly:

- what your **inputs** and **outputs** are;
- the **data type** of each (categorical vs. numerical, and ordinal vs. nominal where it matters);
- what **transformations and cleaning** you performed and why — missing values, one-hot encoding, normalization or standardization, thresholding, outliers, class imbalance.

**Identifiers are never inputs.** A row ID, a permit number, a customer code, a URL or a name is not information about the case — it is a label for it. Including one is a straightforward error, and several datasets in the pool contain columns designed to tempt you.

**Feature leakage.** For every input feature, ask: *would this value actually be known at the moment the prediction has to be made?* Features recorded **after** the outcome — or derived from it — must be removed and the removal justified in the report. A model that quietly uses a post-outcome feature looks excellent and is worthless. The test is chronological, not statistical: if you are predicting whether a loan will default, the applicant's income and credit score are known when the loan is approved and are legitimate inputs, while the number of missed payments, the collections flag and the recovery amount are all recorded *after* the outcome you are trying to predict and are not. A feature that is strongly predictive for no reason you can explain is the usual symptom — check its timing before you celebrate it. **Naming at least one feature you dropped for this reason is required.**

**Split discipline.** Perform a train/test split or cross-validation, and fit every transformation (scaler, PCA, imputer) **on the training data only**. Fitting a scaler on the full dataset before splitting leaks test-set information into training. Inside cross-validation this must happen per fold — that is what `sklearn.pipeline.Pipeline` is for.

**Pipeline diagram.** Show the flow of information from raw input to final output as a diagram, as demonstrated in class. It must make clear what goes in, what the stages are, and what comes out.

### 5.4 Evaluation

**For the predictive question:**

- Use **the right metric for the task** — RMSE or MAE for regression, a confusion matrix and its derived metrics for classification.
- **Accuracy alone is not sufficient.** Address class imbalance and choose a classification threshold deliberately, with an argument for the cutoff you picked.
- **Diagnose the fit.** Is the model overfitting, underfitting, or fitting well? Show the evidence.
- **Tune at least two hyperparameters**, and say how you tuned them (manual sweep, grid search, cross-validated search).
- **Compare your two methods** on the same metric, on the same split, and say which you would deploy and why.

**For the descriptive question**, "evaluation" means showing the structure you found is real rather than imposed:

- **Match the method to the data type.** PCA, hierarchical clustering and k-means with Euclidean distance are defined for **numeric** features. One-hot encoding a categorical column and feeding it to Euclidean k-means is not a neutral convenience — it silently asserts that every pair of categories is equidistant. If your descriptive question is really about categorical data, either restrict to the numeric features and say so, or use a method built for the job (Gower or Jaccard distance, k-modes, k-prototypes). Whichever you pick, justify it.
- Justify the number of components or clusters you chose — a scree plot, an elbow, a silhouette score, or a stability check.
- Show that the result is not an artefact of scaling. PCA and k-means both change completely on unscaled data; demonstrate you know which you used and why.
- **Say what the components or clusters mean** in the language of the data. A cluster you cannot describe in words is not a finding.
- If the structure is weak — the clusters overlap, the variance is spread across many components — **say so**. That is a legitimate and interesting result, and it scores better than a forced segmentation.

### 5.5 Interpretation

Do not just report numbers.

- Report the **findings and insight** the numbers convey, in plain English that anyone in the room can follow. In your career you will be explaining this to people who do not know what an F1 score is.
- Use **visualizations** where they help you understand the data or communicate the result. **Every figure you show, in the report or on a slide, must have:** axis labels and a legend where applicable; a **one-line caption saying what the reader should conclude from it**; and, if it is complex, a pointer to the part that matters. A figure without a takeaway is decoration.
- Tell the **story of how the model improved** — what you tried, what failed, what you changed, what it bought you. A project that reports only the final number is missing the most interesting part.

---

## 6. Deliverables

All submitted through Blackboard.

### 6.1 Written report — due Mon Nov 23, 11:59 PM

- **A single PDF.** Times New Roman, 12 pt, 1-inch margins.
- **Maximum 10 pages** for the main body, excluding the cover page and appendix. The appendix has no page limit — put extended discussion, secondary figures, and sources there.
- One report per team.

**The report must be self-contained.** If a claim needs a figure or a number to be understood, that figure or number belongs in the report or its appendix. **We will not open your notebook to find something the report left out** — anything missing is simply missing, and is marked as such.

**Two sections are required in every report:**

- **Limitations.** What might be wrong, uncertain, or sensitive to a choice you made? What was inconclusive? What would you do with more time or better data, and why? A report with no limitations section reads as a report whose authors did not look for any.
- **Contribution table.** One row per team member, listing the concrete technical tasks that person personally carried out and which methods they ran (*"cleaned the missing-value columns and tested median versus drop"*, *"ran the k-means sweep for k = 2–8 and produced the silhouette comparison"*). Plain English, no jargon, no vagueness. **Writing slides, editing prose, and coordinating the team do not count as technical contribution** — those are expected of everyone and are not what this table records. Each row must also **name the specific files or notebook sections** that person wrote, so the table can be checked against the comments in the code and the repository's commit history (§6.3).

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
- Submit to Blackboard: the `.ipynb`, and the repo link. The pool datasets are public, so a link is enough — do not upload raw data unless you modified it, in which case include the modified file.

#### Attribution — three layers, and they must agree

1. **A comment at the top of every section you wrote**, naming you:
   `# --- Priya: preprocessing, missing-value handling, imputation choice ---`
2. **Your own commits** in the team repository.
3. **The contribution table** in the report (§6.1).

> **Putting your name on a section is a claim you will be asked to defend.** If you are asked in Q&A about a block of code with your name on it and cannot explain what it does and why you did it that way, that is worse than not having claimed it — it is a statement about the work that is not true. Claim what you did; do not claim what you did not.

> The repo does not relax the self-contained rule in §6.1. The report is graded on what the report contains; the repo is how contribution and reproducibility are checked.

> **Resubmission:** if you update a submission, you must re-upload **all** files — earlier submissions are discarded and only the final submission is graded.

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

**Deliberately leave out** of the talk: your preprocessing steps one by one, every hyperparameter you swept, every chart you made, and the code. Those belong in the report, and we will ask about them in Q&A. A team that spends two minutes on one-hot encoding has spent two minutes not making its argument.

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

**What scores poorly:** an answer that repeats a slide instead of addressing the question; a technical term used without being able to unpack it; and any claim you cannot trace back to something in your notebook.

### How Q&A runs

The **first two questions come from your classmates**, not from the instructor. The instructor asks after that.

**You will not be cold-called** — in this session or any other. Participation in BA305 is something you offer, not something extracted from you: see the participation policy in the syllabus. A substantive question put to another team is exactly the kind of contribution it asks for.

Q&A is not a cross-examination and it is not about typos. It is a professional conversation about a piece of work, which is what these conversations look like after you graduate.

## 8. Grading rubric — 100 points

This rubric scores two things: **whether you understood what you were doing**, and **whether you achieved the goals you set**.

It does not score whether you produced a checklist of artifacts. The requirements in §5 are the **floor, not the target** — doing all of them mechanically, with no evidence of understanding behind the choices, is an *Acceptable* project, not a good one.

### How each item is scored

Every item uses the same five levels, and the levels describe **understanding**, not effort or volume:

| Level | % of item | What it means |
| --- | --- | --- |
| **Excellent** | 100% | Correct, and justified with reasoning that shows why the alternatives were worse. The understanding is visible without anyone having to ask for it. |
| **Good** | 85% | Correct, and justified when asked. Minor gaps. |
| **Acceptable** | 65% | Defensible, but the reasoning is thin, generic, or borrowed. The work was done; the thinking is shallow. |
| **Weak** | 40% | Present, but the reasoning is missing, wrong, or contradicts what the code actually does. |
| **None** | 0% | Not attempted, or attempted in a way that shows the idea was not understood. |

### The items

| # | Item | Pts | The question we are actually asking |
| --- | --- | --- | --- |
| 1 | **Goals — are they real, and are they yours?** | 10 | Are your two questions specific, answerable from this data, and worth answering? Can you say who would act on the answer and what they would do differently? Everyone starts from the same pool, so the question **is** the differentiator: a question lifted off the obvious column scores below one that took thought. |
| 2 | **Method choices — do you know why you made them?** | 15 | Are the methods suited to the questions, and can you say why *these* rather than the alternatives you rejected? Naming a method is not the same as choosing one. |
| 3 | **Validity — do you know whether to believe your own results?** | 20 | Leakage identified and removed with reasoning; transformations fit on training data only; the right metric for the task; class imbalance and threshold handled deliberately; overfitting or underfitting diagnosed **with evidence** rather than asserted. This is the heaviest item, because a result that cannot be believed has achieved nothing. |
| 4 | **Achievement — did you answer your questions?** | 15 | Did you reach an answer for each question, and do you know how good that answer is? **A model that performed poorly is not a failed project.** Honestly establishing that a question *cannot* be answered well from this data — with the evidence, a diagnosis, and what it would take to do better — earns full marks here. Quietly swapping in an easier question, or reporting only the run that worked, earns none. |
| 5 | **Interpretation and communication** | 20 | Do the report and the talk explain the *why*, not just the *what*, to someone who does not know what an F1 score is? Did you prioritize the argument over the detail in the 7 minutes you had? Do the visualizations carry the finding honestly? |
| 6 | **Defense and ownership** | 15 | In Q&A: can **any** member explain **any** part of the work? Honest uncertainty — *"we don't know, and here's how we'd find out"* — scores above a confident guess. A bluff scores below silence. |
| 7 | **Reproducibility** | 5 | Does the notebook run top to bottom from a fresh runtime, and can a classmate follow it? |

**Item 7 carries more weight than its 5 points suggest.** If your code does not run, your results **cannot be verified**, and item 3 (Validity) is capped at *Weak* — a swing of up to 12 points. Restart your runtime and Run All before you submit.

**There is no bonus.** Work beyond the course content is welcome, and it shows up where it belongs — in items 2, 4 and 5 — but it never compensates for a project that is not sound. Complexity is not a credential.

### What a strong project looks like

- Curiosity — you wanted to know the answer.
- Clear explanations, in plain language.
- Explicit about how the course material helped, and where it fell short.
- Lessons learned beyond the syllabus.
- Unexpected problems, reported honestly and shared with the class.
- A real account of what was different going from a classroom exercise to a real project.

### What a weak project looks like

- Copy/paste from an online notebook, from a chatbot, or from lecture material.
- No curiosity to explore anything.
- Overly complex or incorrect explanations.
- No real analysis — a model fit, a number reported, nothing interpreted.
- A clean-looking result with no account of what was tried and discarded.
- Visible lack of effort.

---

## 9. Generative AI

The full policy is in the syllabus. For this project specifically:

- **Your report and slides must be written entirely by you, in your own words.** Using Generative AI to write prose for the report or slides is prohibited.
- **If you use Generative AI to assist with code, you must explicitly label every such block** and disclose it in the required appendix — tool and version, how it was used, and links or screenshots of the exchange.
- **You are fully responsible for everything you submit.** AI-generated errors and hallucinations are your errors.
- The instructor may ask you to explain any part of your work. **Inability to explain your own submission in a way that demonstrates understanding and ownership is treated as evidence that the work is not yours**, and is handled under the Academic Conduct Code.

Any violation of the AI policy is treated as a serious honor code violation.

---

## 10. Late policy

**10% of the project grade for each midnight that passes after the deadline**, applied to every dated project item — team registration, the proposal, the slides, and the report — with one distinction between them:

> **The written report** is capped at a **20%** deduction, beyond which it receives a **zero**. A report more than two days late is not accepted.
>
> **Team registration, the proposal, and the slides** are capped at a **30%** deduction and are still expected. The deduction stops growing at 30%, and a deliverable never submitted at all takes the full 30% *and* forfeits its feedback and the points for its content.

Each item's deduction is applied once, to your project grade. For the slides, "the deadline" means **11:59 PM the night before your own slot**, not the night before the first presentation session.

---

## 11. Where to ask

**Piazza is the only contact channel for this course.** Post project questions there so the whole class benefits; mark it private if it concerns your team's specific data. Office hours are the right place for anything that needs a screen share.
