# COM1001: Introduction to Software Engineering &mdash; 2024/25 Spring Semester

Welcome! This repository contains information, slides and practical sheets, to support the Spring Semester of the COM1001 module "Introduction to Software Engineering" at the University of Sheffield.

Jump to:
* [1. Primary Teaching Staff](#1-primary-teaching-staff)
* [2. Getting Started](#2-getting-started)
* [3. Schedule and Resources](#3-schedule-and-resources)

## 1. Primary Teaching Staff

  |<img src="./misc/phil.jpg" width="150"/> | <img src="./misc/donghwan.jpg" width="150"/>|
  |:----------------------------------------:|:--------------------------------------------:|
  | [Phil McMinn](https://philmcminn.com) <br /> Lectures & Practical Sessions | [Donghwan Shin](https://www.dshin.info) <br /> Team Project |

## 2. Getting Started

All of the materials for the module this semester will appear in this repository rather than being uploaded to Blackboard.

You can download the content directly from this page, or preferably you can clone it to your device using the following command in your terminal:

```console
git clone https://github.com/UoS-COM1001/com1001-2024-25-spr.git
```

You need to get Codio setup so that you can develop your team project and run the code examples in a further repository the [COM1001 examples repository](https://github.com/UoS-COM1001/com1001-examples). To do this, follow the instructions on the [Getting Started](./getting-started.md) page.

If you **encounter technical problems or issues**, you'll need to consult the [Technical FAQ](technical-FAQ.md). Importantly, this page tells you what to do if your particular question or issue is not specifically addressed by the FAQ itself.

The [Group Project Brief](Spring-Project-Brief.md) will give necessary details about your group project and assessments. If you have any questions regarding that, please consult the [Project FAQ](project-FAQ.md) and use the Discussion Board/Forum.

## 3. Schedule and Resources

Materials for the module can all be found in this repository, which consists of directories corresponding to content for each week. Files will be added as we proceed through the module. You can clone this repository to your machine to get all the materials automatically, rather than having to download them each time &mdash; just ensure that you regularly do a `git pull`.

Lecture and practical content for this module is front-loaded in weeks 1&ndash;5 so that you have all the knowledge and expertise that you need to complete development and testing of the team project in the remainder of the semester.

| Week | [Lecture Content](#lectures) | [Practical Session](#practical-sessions) | [Scrum Meeting](#scrum-meetings) | [Deadline](Spring-Project-Brief.md#assessment) |
|-:|-|-|-|-|
|1     | **Introduction**<ul><li>[Introduction to Semester&nbsp;2](slides/0-1-introduction.pdf)</li><li>[Semester 2 Group Project](slides/0-2-group-project.pdf)</li></ul>**Foundations**<ul><li>[Web servers and HTTP](slides/1-1-webservers-and-http.pdf)</li><li>[An Introduction to Sinatra](slides/1-2-sinatra.pdf)</li><li>[Controllers](slides/1-3-controllers.pdf)</li><li>[Views](slides/1-4-views.pdf)</li><li>[Queries](slides/1-5-queries.pdf)</li></ul>| <ul><li>[Starting to Develop Your Team Web Application](practicals/week1.md)</li><li>[Coding Challenge](challenges/week1.md)</li></ul> | Team Operating Agreement | |
|2     | **Forms & Sessions**<ul><li>[Forms &mdash; the basics](slides/2-1-forms.pdf)</li><li>[Sanitisation & Validation](slides/2-2-sanitisation-and-validation.pdf)</li><li>[GET and POST](slides/2-3-forms-get-and-post.pdf)</li><li>[Sessions](slides/2-4-sessions.pdf)</li></ul> | <ul><li>[Queries and Forms](practicals/week2.md)</li><li>[Coding Challenge](challenges/week2.md)</li></ul> | Sprint 1 | |
|3     | **Databases**<ul><li>[Databases](slides/3-1-databases.pdf)</li><li>[Object Relational Mapping](slides/3-2-orm.pdf)</li><li>[Data Confidentiality](slides/3-3-data-confidentiality.pdf)</ul> | <ul><li>[Creating a Database and a Set of Models for Your Application](practicals/week3.md)</li><li>[Coding Challenge](challenges/week3.md)</li></ul> | Sprint 1 | |
|4     | **Testing**<ul><li>Why Write Automated Tests?</li><li>Writing Automated Tests with RSpec</li><li>Test Scope</li><li>Unit &amp; Integration Testing of Web Applications with RSpec</li><li>Acceptance Testing with RSpec</li><li>Test Coverage</li></ul> | <ul><li>Testing Your Application</li></ul> | Sprint 2 | |
|5     | **Development Issues**<ul><li>Debugging</li><li>Refactoring</li></ul> | <ul><li>Coding Standards and Refactoring</li><li>Debugging Challenge</li></ul> | Sprint 2 | |
|6     | *No lectures* | Drop-In Session | Sprint 3 | |
|7     | *No lectures* | Drop-In Session | Sprint 3 | Formative <br /> Friday (28 March) 3pm |
|8     | *No lectures* | *No practical session* | Sprint 4 | |
|Easter|
|9     | *No lectures* | Drop-In Session | Sprint 4 | |
|10    | *No lectures* | Drop-In Session | Sprint 5 | |
|11    | *No lectures* | Drop-In Session | Sprint 5 | Summative <br /> Friday (16 May) 3pm |

### Lectures

Lectures will be held on **Tuesday 9&ndash;11am and Thursdays 4&ndash;5pm in the [Diamond](https://www.sheffield.ac.uk/engineering/diamond-engineering/floor-plans), lecture theatre 1** in weeks 1&ndash;5. There will be a break during 2 hour lectures, and also a (non-assessed) team quiz. There will be a prize in week 5 for the team that performs best overall in the quizzes.

### Practical Sessions

Practical sessions will be held on **Thursdays 5&ndash;6pm in the [Diamond](https://www.sheffield.ac.uk/engineering/diamond-engineering/floor-plans)**.

#### Weeks 1&ndash;5

In weeks 1&ndash;5, the practical sessions consist of team exercises, coding challenges, and will offer practical technical help regarding the team project. You will need to bring your own laptop to this session, or use the laptop loan facility.

Where you go and where you sit depends on which team you're in:
* **Teams 1&ndash;23** need to go to **Computer Room 3** on the second floor, and follow the [seating plan for CR3](misc/cr3-practicals.pdf).
* **Teams 24&ndash;47** need to go to **Computer Room 5** on the ground floor, and follow the [seating plan for CR5](misc/cr5-practicals.pdf).

#### Weeks 6&ndash;11

In weeks 6&ndash;11, the practical session will take the form of an (optional) drop-in session. Here, you can talk to us about any technical problems you're experiencing with your code, or ask any other question you like (e.g., re-explaining lecture content) and we'll endeavour to help. This will take place in **Computer Room 3**. The whole room will be reserved so you can use the space to work simultaneously in your teams.

### Scrum Meetings

Each team will have timetabled scrum meetings once a week, **starting in week 1 and finishing in week 11**. These meetings will happen on **Tuesday afternoons between 2-3pm in Computer Room 3 (second floor) or Computer Room 5 (ground floor)** of the Diamond. Check out the [seating plan](misc/cr3-cr5-scrum-meetings.pdf) to find out where you need to be.

Each team will be allocated a supervisor (a member of the department's teaching staff). Your team supervisor will check-in with you to see how your project is going during the scrum meetings. See the [Team Project Brief](Spring-Project-Brief.md) for more details.

Note: your team supervisor will focus on monitoring your progress and teamwork, *not* providing technical advice on your project. Technical advice will be available (via the demonstrators) in the scheduled practical sessions listed above.
