# Week 5: Coding Standards and Refactoring

Important to any software engineering team is the existence of an agreed set of
coding standards. Coding standards are a set of guidelines, best practices,
programming styles and conventions that developers adhere to when writing source
code for a project. Most software companies have them. Coding standards set out
how you will format your code, to reduce disagreements over — for example — how
many spaces you should indent your code by.

So-called "linting" tools help enforce coding standards. Linting tools, or
linters, for short, automatically check your source code for programmatic and
stylistic errors. You may have already met `Rubocop`, one such tool for Ruby.

Rubocop checks for (and can automatically correct) stylistic errors. Rubocop
involves different "cops" — program style rule checkers — for assessing your
code for places where these rules are broken (so-called "offenses").

### 1. Start using Rubocop for your project

You can decide to override some of the things Rubocop complains about with a
`.rubocop.yml` file in the directory of the code you're checking. Note that the
`code` directory of the `com1001` repository contains several examples of these
files — look in almost any code directory and load one up.

### 2. Refactor!

Rubocop will likely complain about many things in your project. Discuss in your
team: which ones will you change (refactor) your code for? There may be some
that you will decide to ignore. (For example, Rubocop likes strings to use
single quotes. You, like me, may prefer double quotes, and decide to turn this
cop off.) Others are more serious, like incorrect stylistic usages of Ruby,
methods that are too long, and so on. Some of these may be auto-correctable
(using the `-A` switch, i.e. by issuing `rubocop -A` at the terminal). Be
careful to commit your code before doing this, because Rubocop will directly
change your code files!

### 3. Database structure

Given the lecture last week, discuss in your teams whether your current database
structure is the best one, and whether you need to do any refactoring to split
tables up into smaller ones, potentially using foreign keys.
