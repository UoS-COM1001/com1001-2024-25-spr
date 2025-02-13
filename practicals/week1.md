# Week 1 Practical: Starting to Develop Your Team Web Application

You should already have your Codio setup by this point, if not, review the
instructions on the [Getting Started](../getting-started.md) page.

Read the rest of this page first, then start to tackle each of the tasks. Don't
leave before doing task 6 &mdash; deciding when and where you're going to meet
next as a team.

### 1. In your teams, start to think about the architectural design of your web application

Take some of your key stories and discuss:

* What pages will be needed?

* What will they look like and do? What forms are needed? (Note that we have not
  yet covered databases, but assume the user will be able to submit data via
  forms that you will be able to store data in a database for use elsewhere in
  the application.)

* How will these pages link together? For example, what will be the overall
  structure of the application, what hyperlinks are required, which pages are
  accessible only via form submissions.

### 2. In terms of the stories you discussed, and the pages you decided upon, and the eventual Sinatra application:

* What routes will be required?

* How might these routes be grouped into one or more distinct controller files?
  (For example, each different part of the system might have its own controller
  file, to keep all functionality for that part of the system together.)

* What views will you need?

* What aspects of these views are "reusable" (e.g., common headers and footers
  in the application) that could form their own `.erb` files included into other
  views (as discussed in lectures).

### 3. Ensure your Sinatra application has been created

This was part of the [Setting up Codio](../setting-up-codio.md) instructions.
Ensure everyone in your team can clone the team repository and that you have run
`create_app` in it, to create the basic files needed for your Sinatra
application.

Make sure that:

* You can successfully set up two or more routes, and can get them working

* You can get each route to utilise a "view"

* You can get one or more views to display images, and use a CSS file placed in
  (or, ideally, in subdirectories of) the `public` directory of the application

* If you create any directories, that they haveat least one file. This is
  because Git will ignore empty directories, and so your intended directory
  structure will get lost. If you have no files to add to a directory right now,
  just add a `README.md` file, with one or two sentences explaining what the
  directory will eventually contain.

### 4. Initial Commit, Push, and Pull

Make sure everyone can `pull` other people's changes, and that they themselves
can `commit` changes and then `push` them.

Now: can each member do a pull and get the latest version of the project?

### 5. Responsibilities

Start to decide how you're going to divide responsibility up for different parts
or aspects of the project. For example, who will be in charge of which stories?
**Make sure that each person has tasks that involve all aspects of development**
– i.e., that you don't have one or two people just programming, another just
testing, another just doing the views and so on. You may, however, want to
assign someone as "quality control" for each of those aspects, making sure they
get done.

### 6. Meeting Schedule

Before you leave, decide how and where you're going to meet-up each week, in
person or online, to continue development on the project.

### 7. Challenges

If you're all done, then attempt this week's
[challenges](../challenges/week1.md).
