# Boston University Questrom School of Business

# BA305 – Business Decision-Making with Data

### Fall 2026

---

## Course Administrative Details

- **Instructor:** [Mohannad Elhamod](https://www.linkedin.com/in/mohannadelhamod/) (Contact exclusively through [Piazza](https://piazza.com/bu/fall2026/ba305))
- **Office hours:** **By appointment only** — request an appointment through Piazza (see the Office Hours policy below)
- **TA:** Aris Johnson (Contact exclusively through Piazza); TA office hours are also **by appointment only**, requested through Piazza
- **Class time and place:** Tuesday / Thursday — **Section A** 9:30 – 10:45 AM, **Section B** 8:00 – 9:15 AM / HAR 404
- **Friday makeup session times:** **Section A** 8:00 – 9:15 PM, **Section B** 6:30 – 7:45 PM / HAR 419
- **Term:** September 2 – December 10, 2026
- **First class meeting:** Thursday, September 3, 2026
- **Last class meeting:** Tuesday, November 24, 2026
- **Number of sessions:** 27 sessions of 75 minutes — 23 regular meetings plus 4 makeup sessions
- **Makeup sessions:** Four sessions meet on a **Friday** — **Fri Oct 2** (session 10), **Fri Oct 16** (session 14), **Fri Oct 30** (session 19), and **Fri Nov 6** (session 22). These meet in the **evening** at the times listed above, in **HAR 419**.

> The instructor reserves the right to update the syllabus at any time.

> **About the makeup sessions.** These sessions fall outside the regular meeting pattern because of the instructor's scheduling constraints, and they substitute for the meetings that would otherwise have taken place in December. They are **not graded for participation** and **carry no graded assessment of any kind**. Their sole purpose is to give you additional time to prepare and review for the assessments that are graded. Attendance is strongly encouraged but is not part of your grade.

### No-class dates

| Date | Reason |
| --- | --- |
| **Tue Oct 13** | **Substitute Monday schedule — BA305 does not meet** |
| **Thu Nov 26** | **Thanksgiving recess (Nov 25 – 29)** |
| **Dec 1, 3, 8, 10** | **No meetings** — replaced by the four Friday makeup sessions. All teaching, both exams, and all project presentations are completed before the Thanksgiving recess. |

---

## Course Description & Learning Goals

This is an advanced analytics course on data-driven decision-making in business environments. Business analytics professionals need to be able to (i) uncover patterns in data (*descriptive analytics*); (ii) use data to make predictions about future outcomes (*predictive analytics*); and (iii) leverage data to make optimal business decisions (*prescriptive analytics*). This course takes a holistic approach, covering all three pillars. We explore data reduction, classification, decision analysis, and optimization, linking data models to strategy through statistical programming in Python. Case studies and a group project apply these topics to practical business problems.

Upon completion of this course, you will have:

- Formulated and identified a business problem and used analytical tools to analyze it
- Structured decisions and estimated the value of information and time
- Quantitatively analyzed decisions that involve optimization in the face of uncertainty
- Acquired advanced analytics knowledge and communicated it to peers
- Presented and communicated a business analytics project

### A note on expectations

This is a technical course taught to a business audience. The material stays grounded in how these methods actually work and where they fail — not in what they are marketed as doing. You will read confusion matrices, write Python, and formulate linear programs. A STEM background is not required, but keeping up with the labs is.

---

## Course Structure & Pedagogy

**Foundational material**

- The data project lifecycle, from framing a question to presenting results
- Data visualization — reading charts, then building them
- Dimension reduction — PCA, plus an introduction to nonlinear methods (t-SNE, UMAP)
- Model assessment
- Classification — k-NN, Naïve Bayes, decision trees, logistic regression, neural networks
- Optimization — linear programming, network models, integer programming

**Group project**

- **Team formation and dataset choice.** Teams form in the first week and are registered on Blackboard by **Thursday, September 10**. The registration also asks each team for its **ranked top three datasets** from the pool in `Project/PROJECT_DIRECTIVES.md`; datasets are allocated and posted on Piazza the next day, **Friday, September 11**. Preferences are honoured where possible, but the class as a whole should not present fourteen versions of the same file, so a team may not get its first choice. Registration carries **no grade of its own**, but it is not optional: a late registration is penalized on the same scale as any other late project submission (see *Late submissions* below), applied to your final project grade. **You do not choose your own data and you do not propose your own topic** — every team works from an allocated dataset, and working out what is worth asking of it is the first part of the project and is graded in its own right. What the project requires is set out in Session 1 and in the `Project/` folder — the two workshops later in the term are progress checkpoints, not the point at which requirements are explained.
- **Project proposal.** Each team submits a short written proposal on Blackboard by **Thursday, September 17** — two weeks into the term. The proposal carries **no grade of its own**; its purpose is to get you written feedback while there is still time to change direction. It is not optional: a late proposal is penalized on the same scale as any other late project submission (see *Late submissions* below), applied to your final project grade.
- **Where to find it.** `Project/PROJECT_DIRECTIVES.md` in the course repository is the single source of truth for the project: requirements, the proposal template, deliverables, the presentation format, and the full grading rubric.
- **Presentations and report.** Each team presents its work to the class in **7 minutes, followed by 8 minutes of Q&A** in which any member may be asked about any part of the project. Presentations run November 12, 17 and 19; slots are assigned from a **ranked-preference poll on Piazza that opens Mon Oct 19 and closes Fri Oct 23**, and a team's **slides are due at 11:59 PM the night before its slot and cannot be changed after it presents**. The written report and the team's **GitHub repository link** are due **Monday, November 23**, four days after the last presentation session; the repository is the whole code submission and is frozen at that deadline.

---

## Course Materials and Logistics

There is no textbook to purchase and no assigned textbook reading.

**Required readings** are short, free, online pieces. They are listed in the *Preparation & Deliverables* column of the course schedule below, and each is also linked from a `Required/` README in that session's folder in the course repository.

**Optional readings** are suggestions for going further. They are never assumed in class and never assessed. Session-specific chapter suggestions appear in the same column of the schedule, and supplementary material is placed in each session's `Optional/` folder in the course repository.

### Software and accounts

All lab work runs in Google Colab in your browser; no local Python installation is required or supported.

- **Google Colab** — free tier; sign up [here](https://colab.research.google.com/signup). **This must be done before the first class** — the schedule does not leave a full class for setup.
- `lab1_python_tutorial.ipynb` — a self-paced Python/NumPy/pandas tutorial in the Session 01 folder of the course repository, **also required before the first class** (\~1.5–2 hours). It is not taught live; class time from Session 03 onward assumes you have run it. One cell raises an error on purpose — that is a teaching example, not a bug.
- **Examplify** — the exam application used for Exam 1 and the Final. Installing it and confirming it runs on your laptop **well before Exam 1** is **your responsibility**; see the assessment details below. Questrom IT is the support channel if you have trouble, and can provide a loaner laptop.
- **Bring a laptop to every session.** Don't forget your power cord.
- **Course GitHub repository** — <https://github.com/elhamod/BA305_Fall_2026>. Slide decks, lab notebooks, datasets, and supplementary material live here. It is public: you do not need a GitHub account to read it, and nothing needs to be downloaded — each notebook opens directly in Colab.
- Blackboard is the administrative hub: announcements, deliverables, and grades. Project deliverables are submitted there.

---

## Course Policies

### Contact Policy

**Piazza is the only channel for course communication.** All questions, discussion, and private messages to the instructor and the TAs go through Piazza. Messages sent by email or through Blackboard will most likely not receive attention.

Join the course Piazza site at [**https://piazza.com/bu/fall2026/ba305**](https://piazza.com/bu/fall2026/ba305) **before the first class**, and do two things straight away:

1. **Use your formal name as it appears on Blackboard**, so your posts and participation can be matched to you.
2. **Turn on at least a daily email digest**, so you do not miss announcements. Click the **gear icon** in Piazza, choose **Account/Email Settings**, then under **Class & Email Settings** click **Edit Email Notifications** for this course, select **Daily Digest**, and click **Save**. ([step-by-step instructions](https://support.piazza.com/support/solutions/articles/48000574383-student-email-notification-settings))

When you post:

- **Address the post to the whole instructor team, not to one person.** In the *Post to* field, select *"All Instructors"* rather than a single name — a post addressed to one person is the most common reason a question sits unanswered.
- **Choose the right post type:** a **Question** when you need an answer, a **Note** when you are sharing a resource or starting a discussion.
- **Post publicly by default.** Use a private post only for something personal — a grade, an accommodation, or a difficulty within your project team. Public questions get answered faster and help everyone.
- **Write a specific title**, say what you have already tried, and paste code and error messages as text rather than screenshots.
- **Search the existing posts first** — your question may already be answered.

New to Piazza? See [how to post a question](https://support.piazza.com/support/solutions/articles/48000574396-students-post-a-question), the [student help center](https://support.piazza.com/support/solutions/48000185443), or this [short video tutorial](https://www.youtube.com/watch?v=j7I_T3p-NPE).

### Office Hours

Office hours — for the instructor and for any teaching assistants — are held **by appointment only**; there is no standing weekly slot. To request a meeting, send a private Piazza message that lists **at least three possible time frames, each at least two hours wide** — for example, "Tue 1:00 - 3:00 PM, Wed 10:00 AM - 12:00 PM, Thu 3:00 - 5:00 PM." Broad windows are what make it possible to find an overlap on the first try; a request naming a single time or a narrow slot rarely lands.

**Requests that do not include three qualifying time frames will not be answered.** You will need to resubmit, which delays the meeting — often past the point where it would have been useful. Plan ahead and send your request well before the deadline you need help with. Meetings are held in the instructor's office (HAR 546D) unless another arrangement is agreed in advance.

### Attendance Policy

Regular attendance and preparation are essential, as class sessions include hands-on activities and discussions that cannot be replicated outside of class. In accordance with Boston University policy and Massachusetts State Law, absences for religious observance are excused. The instructor should be notified in advance when possible.

Because in-class activities and discussion are central to this course and cannot be replicated afterward, your attendance and preparation are reflected in your participation grade (see the Course Evaluation & Expectations section below).

- **Four sessions meet on a Friday evening** — **Fri Oct 2**, **Fri Oct 16**, **Fri Oct 30**, and **Fri Nov 6** (Section A 8:00 – 9:15 PM, Section B 6:30 – 7:45 PM, HAR 419) — in place of the December meetings. They are not graded for participation and carry no graded assessment; see *About the makeup sessions* above. Please put all four on your calendar now and raise any conflict with the instructor in the first two weeks of the semester.
- There is no separate attendance rule and no fixed number of permitted absences. Attendance matters only through participation: participation cannot be earned in a session you are not present for, so students who miss a substantial number of sessions will find it difficult to score well on that component.
- Other assessments and in-class participation evaluation are not waived or postponed due to absence. Both exams are administered in class via Examplify on your own laptop. There are no makeup sittings as a matter of course; a **documented** medical or University-excused absence may be granted a makeup sitting at the instructor's discretion, arranged through Piazza **as early as possible** and normally before the exam. An undocumented absence from an exam receives a zero.

### Academic Accommodations for Students with Special Needs

In keeping with university policy, any student with a disability who needs or thinks they need academic accommodations must contact Disability & Access Services at 617-353-3658, or visit 25 Buick Street, Suite 300, to arrange a confidential appointment with a staff member. Accommodation letters must be delivered to your instructor in a timely fashion — within two weeks of the date on the letter, and not later than two weeks before any major examination. While reasonable requests will be accommodated when possible, please note that accommodations may still not be delivered absent an official letter of accommodation.

### Academic Conduct

Please refer to the [university's general academic integrity policy](https://www.bu.edu/provost/students/undergraduate/academic-integrity/) and [code of conduct](https://www.bu.edu/academics/policies/academic-conduct-code/). Unless specifically instructed to the contrary, these policies will be enforced, and the procedures of BU's Academic Conduct Code are followed wherever there is clear evidence of a violation.

- **Assessments.** Cheating includes any copying or sharing of answers, or any attempt by a student to alter their own or another student's performance on an assessment in violation of that assessment's stated or commonly understood ground rules. Use of electronic devices or supplemental material that is not explicitly allowed is also a violation.
- **Coursework and projects.** Copying another student's or team's files, data, or project — including from a previous year — and representing the work as your own is a violation, as is copying the exact wording of another write-up. Where there is reason to believe that part of a submission was copied, it will receive a zero pending review.
- **Course materials.** Posting course material of any kind — assessments, slides, notebooks, or completed projects — to the web is expressly prohibited. This includes crowd-sourced platforms such as Course Hero and SlideShare.
- **Citations and references.** For all submissions, citations and references to any articles, repositories, or other materials used are required. Omission will lead to losing points, and non-compliance constitutes a violation of the honor code that will result in appropriate disciplinary action.

### Use of AI

**Where Generative AI is permitted in this course.** Generative AI may be used in support of the term project, subject to two conditions that apply together: any use of genAI (ChatGPT, Claude, Gemini, or similar) that aids or enhances your project must be **fully disclosed at submission**, and **every member of the team must be able to explain and defend any AI-assisted work as their own** — what it does, why it was chosen, and why it is correct. Work you cannot explain will not receive credit, whether or not it was disclosed. [Terrier GPT](https://terriergpt.bu.edu/login) is free to you as a BU student and is one option among others; it is not endorsed or required, and using it carries exactly the same disclosure and defence obligations as any other tool. Exam 1 and the Final are closed-book and administered in a locked-down Examplify session with no internet access, so no AI tools of any kind can be or are permitted during them; Colab's AI features must be turned off during in-class assessments. Failure to disclose AI use will result in serious consequences, up to and including failure of the course. You are responsible for adhering to the expectations set for each assessment.

The intellectual growth gained from working through a difficult problem and discovering the answer for yourself cannot be replicated by reading a pre-generated answer. It is important to understand the fundamentals of writing and "thinking" in code before introducing code generated by AI assistants.

**Requirements for use.** Wherever an assessment explicitly allows Generative AI (e.g., ChatGPT, Gemini, Claude, GitHub Copilot), all of the guidelines below must be followed.

**Attribution & transparency:**

- Clearly identify all AI-generated content, even if it was only used for idea generation or editing.
- In-text citations or footnotes should reference the AI tool and the prompt used.

**Required appendix.** Each submission using AI must include a short appendix that contains:

- The specific tools and versions used (e.g., ChatGPT-4.1)
- A brief description of how the AI was used (e.g., brainstorming, coding assistance, debugging)
- The full exchange with the AI tool in the form of weblinks or screenshots (relevant parts may be highlighted)

**Accuracy & responsibility.** AI tools frequently generate incorrect or fabricated facts, citations, or code. You are fully responsible for verifying the accuracy of all AI-assisted content. Any errors or hallucinations will be treated as your own. The course closes with a worked example of exactly this failure mode: an AI-generated optimization model that is confidently, expensively wrong.

**Using Generative AI tools to generate plain English writing is strictly prohibited.** All written work must be created in your own words — that includes a paragraph you then edit and a bullet list you then turn into sentences. If the sentence started as the model's, it does not belong in your submission. **Light grammatical correction is permitted** — spelling, punctuation, agreement, a clumsy clause straightened out, the kind of thing a spell-checker does. The thinking, the structure, the argument and the wording must be yours. Using Generative AI for **ideation and for code** remains permitted, subject to the labelling and disclosure requirements above.

Any submission that violates these requirements may be treated as a violation of academic integrity and will be handled in accordance with the Academic Conduct Code. The instructor reserves the right to call you to office hours to discuss your submitted work and determine whether you understand it or simply copy-pasted it from a Gen AI tool. AI should deepen your understanding, not replace it. You are expected to remain intellectually engaged and responsible for the content you submit.

> **Note:** The type of tool does not change these requirements. "Generative AI" includes not only standalone tools like ChatGPT, Gemini, and Claude, but also GenAI tools embedded within coding platforms (e.g., GitHub Copilot, Google Colab, or VS Code extensions).

To help clarify expectations, here are some examples:

- ✅ **Acceptable:** Asking an AI assistant to explain why a constraint makes a linear program infeasible, then citing it in your report.
- ❌ **Unacceptable:** Pasting the project brief into an AI assistant and submitting the returned model without understanding or citing it.

**Collaboration.** The goal of this course—and of your education more broadly—is to prepare you for real-world success. Given the importance of teamwork and communication in business and analytics roles, student discussions are encouraged. You are encouraged to discuss the course material and your project with others in BA305, but your team must write its own report and construct its own code. You may discuss general concepts, methods, and high-level strategies, but you may not share or view another team's code, written answers, or specific solution details. You are still expected to fully understand, explain, and take ownership of any work submitted under your name. You must be able to discuss and defend your code, analysis, and conclusions when asked. Any help or collaboration—whether from classmates, tutors, or AI tools—must be clearly cited in your submission. Failure to adhere to these guidelines may constitute a violation of the Academic Conduct Code.

- ✅ **Acceptable:** Discussing with another team which evaluation metric suits a class-imbalanced problem.
- ❌ **Unacceptable:** Copying or closely mimicking another team's notebook or write-up, even with small modifications.

### Professional Conduct Policy

- **Bring your laptop:** You will need it for in-class coding in nearly every session. Don't forget your power cord.
- **Laptops open for coding only:** Screens are open during hands-on coding activities and closed during discussion, demos, and lectures. For notetaking outside coding activities, please use a paper notebook or a tablet with a pen (no keyboards).
- Cellphones are prohibited unless specifically allowed by the instructor for certain in-class activities.
- Activities unrelated to class — social media, news sites, video, gaming, email, messaging — are not permitted at any time.
- **Place your name tent:** This helps your instructor learn your names, and it is needed so that your participation can be recorded. Please use your formal name as shown on Blackboard.
- **Pay attention to whoever is speaking:** whether that is the instructor or a fellow student presenting. See *Class participation* below for what happens when it is clear you were not.
- **Punctuality:** Students are expected to arrive on time.
- Food is not allowed. Drinks are OK if consumed in an undistracting way.
- **Violations:** The first violation of any of these policies will incur a warning. Subsequent violations will warrant losing 1 point of the final course grade per citation.

### Diversity & Inclusion

This course is developed with attention to how identity and culture shape its content. Throughout the term, the emphasis is on knowing where your data came from, and how and why it was collected, so that potential sources of bias can be recognized. Perspectives related to the course content are invited. If there are topics that would benefit from additional social context or a differing perspective, let your instructor know, and resources and opportunities will be sought to bring a wider range of perspectives into the classroom.

### Sexual Misconduct / Title IX

The Questrom School of Business is committed to fostering a safe learning environment and preventing sexual misconduct. All forms of sexual misconduct — including rape, acquaintance rape, sexual assault, domestic and dating violence, stalking, and sexual harassment — violate BU policy, whether they happen on or off campus. Title IX of the Education Amendments of 1972 prohibits sex-based discrimination in federally funded education programs. If you or someone you know has been harassed or assaulted, resources are available at <http://www.bu.edu/safety/sexual-misconduct/>.

---

## Course Evaluation & Expectations

For details on Questrom's program-wide guidelines for grading, please refer to the [provided link](https://www.bu.edu/academics/questrom/policies/grades-and-course-credits/). Questions about a grade received on a particular assessment must be raised within one week of receiving it; otherwise, the grade may not be revised. If you have particular grade-related considerations that you think are important, please raise these with your instructor as early as possible (during the first half of the semester at the latest), so that your instructor can help you approach the course in a way that will help you achieve your best possible performance.

The relative weight of assessments in your course grade is as follows:

| Component | Weight |
| --- | --- |
| Class participation | 20% |
| Exam 1 (in class, Tue Oct 6) | 20% |
| Final (in class, Tue Nov 3) | 30% |
| Term project (group) | 30% |
| **Total** | **100%** |

**Class participation (20%).** This grade reflects active, quality contribution to in-class work and discussion. You are expected to arrive prepared to engage with the material critically — being present is not the same as participating.

**Cold-calling is not how this course is run.** Participation is something you offer, not something extracted from you, and the plan is never to put you on the spot. The one situation in which the instructor will call on a student directly is when that student is plainly not following the class — distracted, disruptive, or in breach of the laptop and phone rules in the Professional Conduct Policy. In exchange, the bar is explicit and it is small:

| Substantive contributions over the term | Participation score |
| --- | --- |
| 3 or more | 100% |
| 2 | 90% |
| 1 | 80% |
| 0 | 70% |

**A contribution counts when it moves the discussion** — a question that identifies a real difficulty, an answer that engages with the substance, a challenge to a claim made in class or by another team, a point raised in a lab or workshop, or a substantive question put to a presenting team. Speaking in order to be recorded as having spoken does not count, and quality is what decides whether something is counted at all rather than being scored separately.

Three contributions across twenty discussion sessions is roughly one a month, and the presentation block alone gives three sessions where every team should be asking questions of another. If you are at zero by mid-semester you will be told.

**Attention is expected of the audience, not only of the speaker.** When the instructor or a fellow student is presenting or leading a discussion, you are expected to be following it. If the instructor asks you a question and it is clear that you were not paying attention, that costs **10 percentage points of your participation grade** — for example, a student who had earned 100% drops to 90%. It applies per incident and **is capped at 20% deduction**, so it can lower a participation grade but can never sink it on its own. This matters most during the project presentation block, where the audience is being asked to carry half the Q&A.

**A tentative participation grade will be shared mid-semester as a form of feedback**, so you have time to adjust. The four Friday makeup sessions are not graded for participation; see *About the makeup sessions* above. Name tents are required in every session so that your contributions can be recorded.

**Exam 1 (20%) and the Final (30%).** Two closed-book, in-class assessments made up of multiple choice, code interpretation, fill-in-the-blank code, and short-answer questions (one to two paragraphs each). **Both are administered via Examplify on your own laptop.** Examplify locks the machine down for the duration: there is no internet access, no interpreter or notebook, and no access to your own files, so **you will not run code during either assessment** — questions ask you to read, reason about, and fill in Python. **No electronic device of any kind** other than the laptop running Examplify may be used or accessible during an assessment — no second laptop, tablet, phone, smartwatch, or **calculator**; any arithmetic required is small enough to do by hand. (This restriction applies to assessments only. During labs and hands-on class activities your laptop is expected, and other devices may be used whenever the instructor explicitly authorizes them.) **It is your responsibility to install Examplify and verify that it runs on your laptop well before Exam 1.** Questrom IT is the support channel for installation problems and can provide a loaner laptop if needed. The instructor does not run a setup check and is not responsible for troubleshooting your machine; a device that fails on exam day is not grounds for a makeup sitting. The Final is held **in class on Tuesday, November 3** — there is no sitting during the University's December examination period.

There are no makeup sittings as a matter of course. A **documented** medical or University-excused absence may be granted a makeup sitting at the instructor's discretion; contact the instructor through Piazza as early as possible, and normally before the exam. An undocumented absence from an exam receives a zero.

- **Exam 1 (Tue Oct 6)** covers Sessions 1–9: introduction and preprocessing, data visualization, dimension reduction, model assessment, k-NN, Naïve Bayes.
- **The Final (Tue Nov 3)** covers Sessions 12–18: decision trees, logistic regression, neural networks, and the advanced analytics exercises.

Because the term ends on November 24, the **optimization block (Sessions 21, 23 and 27) falls after both assessments and is not examined.** It remains required material: you are responsible for it in class, and it is fair game for your project.

**Term project (30%).** The project gives you hands-on experience developing a real analytics project and explaining an advanced technique to your peers. **Teams are expected to be four students.** You form your own teams; if the class size leaves a group who cannot form a team of four, come and talk to us and a different team size will be agreed for that group. Every team works from a dataset allocated from a fixed pool; the questions you ask of it, and the methods you bring to them, are yours to choose and to defend. You will present in the presentation block and hand in a written report and your team's repository link on **Monday, November 23**, four days after the last presentation session. **There is no weekly homework in this course.** In its place, your team is responsible for making sure the project progresses steadily from the time teams are formed — the two workshops (Sessions 14 and 22) are progress checkpoints on work already underway, not the point at which the work should begin. A team that starts building in November will not have time to recover from anything that goes wrong. **Late submissions.** Project deliverables lose **10% of the project grade** for each midnight that passes after the deadline. For the **ungraded** items — team registration, the ranked dataset choice, and the proposal — the deduction is **capped at 30%**; an item never submitted at all takes the full 30% and forfeits its feedback. For the **graded** items — the slides and the written report — the deduction is **not capped** and keeps growing, so a deliverable ten days late costs you the entire project grade. The full requirements, the deliverables, the presentation format and the **complete grading rubric** are in `Project/PROJECT_DIRECTIVES.md` in the course repository. That document is the single source of truth for the project. Each student is expected to fully grasp, discuss, defend, and take ownership of the entire project, so all team members must actively engage in various aspects of the work, including research, coding, documentation, and presentation.

---

## Other Logistics

**Blackboard usage.** Though several learning platforms and tools are used in this class, Blackboard acts as the hub from where all information can be found. All deliverables and their deadlines are posted through Blackboard. It is essential that you pay close attention to Piazza announcements, which contain critical information, and course materials are updated regularly. While a weekly announcement is generally sent as a reminder, it remains your responsibility to set up your alerts appropriately for any updates in the schedule or reading materials.

---

## Course Schedule

> Note that while the following table provides a holistic overview of the course's schedule, it is only meant to give general guidance. The exact dates, topics, readings, and deliverables will be posted on Blackboard. Whenever there is a conflict between the syllabus and Blackboard, Blackboard is correct.

Sessions are 75 minutes. Rows marked *(makeup session)* are not on the regular Tuesday/Thursday grid: they meet on a **Friday evening** — **Section A** 8:00 – 9:15 PM, **Section B** 6:30 – 7:45 PM — in **HAR 419**.

Optional-reading abbreviations used below: **DMBA** = *Data Mining for Business Analytics* (Shmueli, Bruce, Gedeck & Patel, Wiley, 2019) · **AE** = *The Analytics Edge* (Bertsimas, O'Hair & Pulleyblank, Dynamic Ideas, 2016) · **DSPP** = *Data Science Projects with Python* (Klosterman, Packt, 2019) · **SMDA** = *Spreadsheet Modeling and Decision Analysis* (Ragsdale, Cengage, 2010). **None of these must be purchased.**

| \# | Date | Learning Objective | Topics & Concepts | Preparation & Deliverables (BEFORE class unless stated otherwise) |
| --- | --- | --- | --- | --- |
| 1 | Thu Sep 3 | **Introduction and course setup.** Place descriptive, predictive, and prescriptive analytics on a single map, and get a working Python environment running. | Logistics and deliverables · **the term project brief and what the proposal must contain** · the three pillars of analytics · data quality and preprocessing · getting Python running | **Required reading:** [Flip Flop: Why Zillow's Algorithmic Home Buying Venture Imploded](https://www.gsb.stanford.edu/insights/flip-flop-why-zillows-algorithmic-home-buying-venture-imploded) (\~7 min) · **Required prerequisite:** work through `lab1_python_tutorial.ipynb` (Session 01 folder, \~1.5–2 hrs, self-paced — it is not taught in class) · Sign up for a free [Google Colab](https://colab.research.google.com/signup) account and confirm you can open and run a notebook · **Optional:** DMBA Ch. 1–2 |
| 2 | Tue Sep 8 | **Data visualization I — reading charts.** Read and critique a chart: say what it is for, and identify how a graphic misleads. | Principles of visualization · what each chart type is for · visualizing multidimensional data · lying with statistical graphics | **Required reading:** [How People Actually Lie With Charts](https://vdl.sci.utah.edu/blog/2023/04/17/misleading/) (\~6 min) · **Optional:** DMBA Ch. 3 · AE Ch. 21.5 pp. 382–388 |
| 3 | Thu Sep 10 | **Data visualization II — building charts.** Build in Python the charts you learned to read, and choose the encoding that carries the finding. | seaborn & matplotlib · Laptop Sales case (groupby, bar, box; how a truncated y-axis distorts a comparison) · WHO case (scatter, hue, categorical vs. sequential palettes, log transforms, regression with confidence bands) · choosing the chart yourself | ***Project teams registered on Blackboard, with ranked top-three dataset choices (ungraded; late = standard project late penalty)*** · **Optional:** DMBA Ch. 3 · AE Ch. 15 pp. 261–274 |
| 4 | Tue Sep 15 | **Dimensionality and PCA I.** Explain why high-dimensional data is a problem, and how principal components reduce it without discarding the story. | Projection intuition · curse of dimensionality · standardization, covariance and eigenvalues · scree plot · profiling and interpreting components · the sklearn API | **Optional:** DMBA Ch. 4 |
| 5 | Thu Sep 17 | **Dimensionality and PCA II — nonlinear methods.** Run PCA on a real dataset, show why scaling changes the answer, and read a t-SNE or UMAP plot without over-reading it. | PCA lab on the *Universities* dataset, scaled vs. unscaled · choosing the number of components · t-SNE and UMAP as neighbourhood-preserving embeddings · why distances and cluster sizes in these plots are not interpretable | ***Project proposal due (ungraded; late = standard project late penalty)*** · **Optional:** DMBA Ch. 4 |
| 6 | Tue Sep 22 | **Model assessment I.** Measure whether a model is any good, and read a confusion matrix cell by cell. | Hold-out and k-fold cross-validation · error measures for numeric prediction · the confusion matrix · cutoffs | **Optional:** DMBA Ch. 5 |
| 7 | Thu Sep 24 | **Model assessment II.** Choose a cutoff that reflects what each kind of error actually costs the business. | ROC and AUC · cost-benefit matrix and optimal cutoff · *diabetes* lab: train/test split, kNN, metrics, threshold sweep | **Optional:** DMBA Ch. 5 |
| 8 | Tue Sep 29 | **k-Nearest Neighbors.** Classify a new case from its neighbours, and choose *k* on evidence rather than by default. | Classification vs. regression · distance and combination functions · voting · choosing *k* · UniversalBank loan-acceptance lab: scaling, k-sweep, predicting a new customer | **Optional:** DMBA Ch. 7 |
| 9 | Thu Oct 1 | **Naïve Bayes.** Apply Bayes' theorem to classify text, and say what the "naive" independence assumption buys and what it costs. | Bayes' theorem · multinomial vs. Gaussian Naïve Bayes · Laplace smoothing · spam-filter lab | **Optional:** DMBA Ch. 8 |
| 10 | **Fri Oct 2** *(makeup session)* | **Exam 1 preparation.** Consolidate Sessions 1–9 and confirm the ground rules for the assessment. | Review across preliminaries, data visualization, PCA, model selection and evaluation, k-NN and Naïve Bayes · exam ground rules: closed book, Examplify, no internet or code execution, multiple choice, code interpretation, fill-in-the-blank code, and short answers of one to two paragraphs | *Makeup session — not graded for participation; no graded assessment* |
| 11 | Tue Oct 6 | **Exam 1.** Demonstrate independent understanding of Sessions 1–9. | In class, closed-book, administered via Examplify; no internet and no code execution; no Generative AI | **Exam 1 (in class)** |
| 12 | Thu Oct 8 | **Decision trees I.** Build a decision tree by hand and say what makes one split better than another. | Building trees by hand · stopping criteria · numeric thresholds · Gini and entropy | **Optional:** DMBA Ch. 9 |
| — | *Tue Oct 13* | *No class — substitute Monday schedule* |  |  |
| 13 | Thu Oct 15 | **Decision trees II.** Recognize an overfit tree and control it, and extend trees to regression and ensembles. | Overfitting and pruning · regression trees · ensembles · loan-acceptance lab | **Optional:** DMBA Ch. 9 |
| 14 | **Fri Oct 16** *(makeup session)* | **Workshop 1.** Show what your team has built so far and get feedback on it while there is still time to act on it. | Progress check against the proposal · what the data actually turned out to look like · where the analysis is stuck · course corrections | *Makeup session — not graded for participation; no graded assessment* |
| 15 | Tue Oct 20 | **Logistic regression.** Model a binary outcome and interpret its coefficients as odds rather than as effects on the outcome itself. | The logistic function and the logit · cutoffs · odds and exponentiated coefficients · multicollinearity · *SystemAdministrators* lab with `statsmodels.Logit` | **Optional:** DMBA Ch. 10 |
| 16 | Thu Oct 22 | **Neural networks I.** Trace a forward pass through a small network by hand, so the model is not a black box. | Perceptron · activation functions · a worked 3-input perceptron · layered feedforward networks · the forward pass · preprocessing and architecture choices | **Optional:** DMBA Ch. 11 |
| 17 | Tue Oct 27 | **Neural networks II.** Fit a network to a regression problem and compare it honestly against a linear baseline, including diagnosing a fit that fails. | Predicting used-car prices · dummy encoding and MinMax scaling · comparing architectures against a linear baseline · recognizing and fixing an undertrained model | **Optional:** DMBA Ch. 11 |
| 18 | Thu Oct 29 | **Advanced data analytics exercises.** Apply the full toolkit to an open-ended, messier problem and defend the evaluation metric you chose. | Applying the full toolkit to an open-ended problem · choosing and defending an evaluation metric |  |
| 19 | **Fri Oct 30** *(makeup session)* | **Final preparation.** Consolidate Sessions 12–18 ahead of the Final. | Review across decision trees, logistic regression, neural networks, and the advanced analytics exercises | *Makeup session — not graded for participation; no graded assessment* |
| 20 | Tue Nov 3 | **Final.** Demonstrate independent understanding of Sessions 12–18. | In class, closed-book, administered via Examplify; no internet and no code execution; no Generative AI | **Final (in class)** |
| 21 | Thu Nov 5 | **Optimization I — linear programming.** Turn a business decision into a linear program, then solve it, and see why intuition alone gets the answer wrong. | Analytics taxonomy · the two-step method (formulate, then solve) · the *Domaine Paul Autard* product-mix case · LP in Python with Pyomo/GLPK | **Optional:** SMDA Ch. 1–3 |
| 22 | **Fri Nov 6** *(makeup session)* | **Workshop 2.** Get feedback on your analysis and your argument before the presentation block. | Project build support · rehearsing the analytical claim and how it will be defended | *Makeup session — not graded for participation; no graded assessment* |
| 23 | Tue Nov 10 | **Optimization II — LP and network models.** Read the feasible region, explain why an optimum sits at a vertex, and scale a formulation up to a network. | The feasible region and vertex optima · shadow prices and sensitivity · the Pfizer 4-plant × 4-DC transportation network | **Optional:** SMDA Ch. 1–3, Ch. 5 |
| 24 | Thu Nov 12 | **Project presentations I.** Present your application and defend your design decisions in response to questions. | 7 min presentation · 8 min Q&A and defense | ***Slides due 11:59 PM the night before your signed-up slot*** |
| 25 | Tue Nov 17 | **Project presentations II.** As above. | 7 min presentation · 8 min Q&A and defense | ***Slides due 11:59 PM the night before your signed-up slot*** |
| 26 | Thu Nov 19 | **Project presentations III** *(Section A)* · **open working session** *(Section B)*. Section A presents; Section B, having finished in Session 25, brings data problems of its own to work through in class. | 7 min presentation · 8 min Q&A and defense · **last presentation session** · *Section B:* bring a dataset or a question you want to try, and we work it through together | ***Slides due 11:59 PM the night before your slot*** · ***Report + code repository due Mon Nov 23*** |
| 27 | Tue Nov 24 | **Optimization III — integer programming.** Formulate a decision with binary variables, and recognize a plausible-looking AI-generated model that is confidently wrong. | Why rounding an LP fails · binary variables · the Google AdWords keyword-slot bidding case · a worked example of an AI-generated model that is off by a wide margin · **last class meeting** | **Optional:** AE Ch. 10 pp. 171–188 · SMDA Ch. 6 |

> **Calendar note:** Sessions 10, 14, 19 and 22 meet on a **Friday**, not the usual Tuesday or Thursday. They are makeup sessions replacing the four December meetings. BA305 does not meet on Tue Oct 13 (substitute Monday schedule) or during Thanksgiving recess (Nov 25–29). The course concludes on Tue Nov 24; there are no meetings in December.
