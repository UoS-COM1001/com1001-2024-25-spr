# **Spring Semester Team Software Project**

## Overview

In the spring semester, each team will implement a web system according to the user stories you collected in the autumn semester. The implementation will follow a mini-scrum framework, a simplified version of an agile software development process. 

### Mini-Scrum Framework

The key principles of the mini-scrum are as follows:
- Incremental development: Build your system in small, manageable increments over multiple iterations (i.e., sprints);
- Collaboration: Work together as a team to deliver a working system that meets the client's requirements.

For each sprint (lasting 2 weeks), your team must:
- Plan what to do (e.g., breakdown user stories into tasks, estimate the time needed for each task);
- Do the tasks;
- Review what you have done.

To facilitate this process, we will have _weekly scrum meetings_ every Tuesday at 2 pm from Week 1 to Week 11. The key activities for the scrum meetings are:
- Electing a scrum master (max 3 mins): Each week, a different team member will be the scrum master (the team leader for the week), responsible for leading the discussion;
- Individual stand-ups (max 3 mins each): Each team member will share what they have done, what they will do, and any blockers they have;
- Team progress review (max 15 mins): Discuss the current progress, any blockers, and adjust the next steps together.
- Planning and reflection: At the start of each sprint, reflect on the previous sprint and plan the next sprint (e.g., major tasks to complete, prioritise tasks, etc.).
- Task management: Use GitLb Issue Boards to manage all tasks, including assignments and due dates. This will help you to keep track of what needs to be done and who is doing what.

### Team Supervisors

During the weekly scrum meetings, your _team supervisor_ will be present to do a 5-minute check-in with each team. Before this, the scrum master (the team leader for the week) must submit a [Google Form](...) summarising any outstanding issues (e.g., conflicts, lack of contribution) that need to be discussed with the supervisor.

### Assessment

| Type | Deadline | Deliverables | Semester Weighting |
| --- | --- | --- | --- |
| Formative | Friday 27 March, 15:00 (Week 7) | Report | 0% |
| Summative | Friday 16 May, 15:00 (Week 11) | Report, 15-min demo recording | 100% |

The summative assessment will be based on the interim report. It is to give you feedback on your progress and to help you improve your system for the final submission. The final submission will be assessed based on the final report and the 15-min demo recording.

After the summative assessment, additional changes to the user stories will be requested to mimic real-world additions/changes from clients. How you handle these changes in the remaining sprints will be part of the final assessment.

Note that the formative assessment is not graded, but it is compulsory. If you do not submit the formative report, you will not be able to submit the summative report.


### Client Questions

You can also use the same discussion board (Forum: Team Project - Client Questions) to communicate with the client, as you did in the autumn semester.


## Team Operating Agreement

Each team must have a **signed team operating agreement**, as explained in Semester 1. The template is available on the Blackboard (click this [link](https://vle.shef.ac.uk/bbcswebdav/pid-7099893-dt-content-rid-51488146_1/xid-51488146_1) or go to Semester 1 -> Course Content -> Lectures weeks 4-6 (Requirements) -> 6-1 Teamwork). It is a living document and should be updated as the need arises throughout the project.

If your team does not have a signed team operating agreement yet, create one as soon as possible. It will set out ground rules for working as a team and serve as an essential baseline in resolving disagreements and conflicts, if any.

## Weekly Schedule

You should schedule stories to implement according to your prioritisation of the client's requirements. However, your implementation plan may also be necessarily constrained by the order in which technical material is covered in lectures and labs. Therefore, check out the lecture schedule and plan the stories you will implement for each sprint accordingly.

Below is a suggested week-by-week list of pointers for your team that you can use to check your plan of action:

| Week | Suggested Activities |
| --- | --- |
| 1 | Meet your team members and supervisor. Complete a Team Operating Agreement. |
| 2-3 | Sprint 1 (views and databases) |
| 4-5 | Sprint 2 (unit tests) |
| 6-7 | Sprint 3 (more implementations and tests, prepare for the summative assessment) |
| 8-9 | Sprint 4 (continue, new requirement changes) |
| 10-11 | Sprint 5 (finalise, prepare for the final assessment) |
| 12 | Don't forget to complete the **peer review** (BuddyCheck) by Friday. |


(stopped here; will continue later)


# Report

Iteration 1/2 reports should include the following information:

- Team ID, members, and the summary of each member's major contributions.
  - A map between each member's name and their GitLab user name, especially if you accidentally made commits under your private emails.
- The exact command(s) needed to install and start your system.
- The exact command(s) needed to run your tests.
- The predefined usernames (e.g., admin1, reader1) for inspecting your system.
  - For each account, the password must be the same as the username.
- A list of all your user stories with their status (e.g., to-do, in-progress, or done) and changes (e.g., modified, removed, or newly added).
  - Please cluster stories about the same type of user.
  - Use colours and highlights to distinguish different statuses and changes, as shown in Figure 1 below.
- What you have done in terms of testing (e.g., unit tests, integration tests, and system tests).
- (Iteration 2 only) What you have done in terms of refactoring.
  - You should present *concrete examples* along with your refactoring *summary* to demonstrate the quality of your refactoring.
  - When you include code fragments, you must use source code colouring, line numbers and a proper caption, as shown in Listing 1 below.
- Your burndown chart, showing progress over all of your stories over each iteration.
- Overall, use figures and tables with clear captions, wherever appropriate.
- (Optional) Please append your team operating agreement signed by all team members to the report as an appendix. This is not subject to assessment, but we will use this as a baseline in resolving disagreements and conflicts, if any.
- (Optional) If you have some internal meeting notes/minutes recording attendees, issues, and task distributions during your internal meetings (not the team supervisor meetings), please append those meeting notes/minutes as an appendix to the report. If needed, you can sanitise sensitive information and keep only the important parts mentioned above.

<img width="600" alt="figure-1" src="https://github.com/UoS-COM1001/com1001-2024/assets/12538465/d9180dc0-9e6a-424a-b679-a67e158425ee">
<img width="600" alt="listing-1" src="https://github.com/UoS-COM1001/com1001-2024/assets/12538465/55180e37-1a7b-41ad-af7c-d7c201525707">


## Code Commits to the Team Repository

At the end of Iteration 1, we may inspect your code, but mostly for clarification.

At the end of Iteration 2, we will look at **the last commit** to the team's repository **before the deadline** for the assessment.

- Ensure all the **necessary files** are committed to your team repository **by the deadline**. Otherwise, you will not receive the mark you deserve.
- We will _not_ check out other repositories (e.g., your personal repository from the last semester, or another Git repository).
- **All members** should be making **regular commits**. We will check that you have been making regular commits – not just one or two commits or a sudden rush of commits just before the deadline.
- We will use **Codio** to run and test your code. Therefore, it is strongly recommended that you develop on Codio; otherwise, you must at least deploy often to Codio as it is the required deployment platform.
- We will use **README** to run and test your code. Ensure that your README is up to date and contains the necessary information to run and test your system.
- Ensure that your `Gemfile` is up to date. If we cannot run your application on Codio due to missing gem information, this will severely negatively affect your mark.
- (Pro-tip) Attempt a **clean install** before your final commit to check whether your system is successfully deployed and running on Codio.

## Live Demonstrations

The demonstration meetings will be held with your supervisors during the standard Team Supervisor meeting times Weeks 7 and 11. In these meetings, you will demonstrate the current state of your system for feedback (as if to the client). For this, you should prepare a **10-minute live demonstration** of your system. If possible, let your supervisor try out your system and get feedback. You will have a few days to update your system for the recording you will upload to your repository by Friday.

Here are some remarks for you:

- Be on time.
- Do a rehearsal before the live demo.
- It's for the client – make it easy to follow.

## Team Contribution

Similar to the last semester, you will be using BuddyCheck to rate yourself and your team members on the following criteria:

1. Attendance and punctuality (to supervisor/your own team meetings, etc.).

2. Ability to work effectively with other team members.

3. Quality of contributions.

4. Timeliness of contributions.

Your final individual mark will be formed from a scaling factor that is applied to your overall team mark. The scaling factor is determined by your own self and peer assessment, and those returned by your team members. 

Note: The Department's Policy on Team-Based Assessments requires evidence to support an individual mark varying by more than +/-15% from the team mark; the evidence considered will include Supervisor meeting attendance/notes as well as Slack/GitHub interactions.

## Marking Criteria

The following table details the criteria against which your team's work will be marked. You will receive a mark sheet containing a table with marks and feedback against the aspects detailed below. Each aspect is marked out of 100. The overall mark is the average of each of the marks for each aspect.

Note: (2) indicates for iteration 2 only, and (1+2) indicates for both iterations.

| **Aspect (iterations)** | **Indicative Criteria** |
| --- | --- |
| Implementation Progress (1+2) | **Iteration 1**: The amount of work completed to date, the extent to which you are on track to delivering a good quality product and the appropriateness of stories implemented in this iteration. <br/> **Iteration 2**: The completeness and quality of your final system. The extent to which it implements the Client's requirements, how usable it is, how polished it is, and the extent to which it crashes and/or throws errors. |
| Code Quality (1+2) | The quality of your code, including good coding principles, such as useful variable names, code comments, etc. The basic organisation of your code into units, and its overall structure. |
| Testing (1+2) | The quality of your automated tests, including unit tests, integration tests, and system tests. The extent to which you have justified the level of coverage that you have obtained. |
| Demonstration (1+2) | The quality of your team demonstration. The extent to which it demonstrates major user stories effectively within the limited time. |
| Report (1+2) | The quality of your team report, the extent to which it details all the requested information, including changes to stories, basic information about using your system etc. |
| Refactoring (2) | The quality of your refactoring. The extent to which your team has clear evidence of refactoring efforts written in the report. |
| Deployment (2) | The extent to which it was easy and straightforward to deploy and get your system running—on the basis of your instructions and the implementation of your deployment process—from Git checkout to the commands needed to start the application. |

## Unfair Means

It is essential to bear in mind the departmental rules on unfair means. Activities such as **plagiarism** or **collusion** will be treated as serious academic offences. This could lead to the award of a grade of zero for your submission.

We will be closely scrutinising submissions to detect such practices because it is important that this team project is a genuine reflection of your own understanding of the module.

To avoid any potential accidental wrongdoings, it is especially important that you do not discuss your solutions with other groups. If you have non-technical questions, please use the discussion board (Forum: Team Project - Non-coding Issues). If you have technical questions, please consult with your demonstrators.

We acknowledge that **Generative AI**, such as Google Bard and OpenAI ChatGPT, can be useful in learning. For example, it is okay to use Gen-AI to try various programming exercises. However, **the use of Gen-AI is prohibited in any of your submissions** subject to the assessment (i.e., the reports and the code commits to the team repository). For example, you must _not_ use the code generated by Gen-AI in the code pushed to your team repository. It is crucial that you learn by doing the project by yourself, and gaining an unfair advantage through the use of Gen-AI in the assessment will be treated as unfair means.
