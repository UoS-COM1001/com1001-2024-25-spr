# Technical FAQ

This FAQ deals with technical (Codio, Ruby, Sinatra etc.) aspects of COM1001. If you have questions about the team proejct, then consult the [Project FAQ](project-FAQ.md) instead.

This FAQ is organised into the following sections. Some questions fit more than one section, so ensure you've properly checked the whole FAQ in case you don't see it.

1. [How to Ask
   Questions](#1-how-to-ask-questions-or-how-to-find-your-own-answers) 
2. [Problems Running Code](#2-problems-running-code) 
3. [Problems with Git](#3-problems-with-git) 
4. [Using Codio](#4-using-codio)

If you're certain your issue doesn't seem to appear on the page, check the next section "[How to Ask Questions](#questions)", first. 

If you think an issue needs to be added to this FAQ, [contact Phil McMinn](mailto:p.mcminn@sheffield.ac.uk).

<!--
Note that this FAQ covers technical issues only.
**If you're experiencing a team issue, or
have a question about the team project**, check out the check the [Assignment
FAQ](https://vle.shef.ac.uk/webapps/blackboard/execute/content/blankPage?cmd=view&content_id=_5820338_1&course_id=_96428_1&mode=reset)
on Blackboard. If this does not answer your question, you should contact your
supervisor, or wait until your next meeting with them.
-->

## 1. How to Ask Questions (Or, How to Find Your Own Answers) 

There are no stupid questions, as the saying goes, but there are definitely *lazy* ones. Sometimes the answer to a question you may have has already been answered in lectures and can easily be found in the slides. But as a general rule, before asking a question, try to find the answer yourself. Finding your own answers is an important skill that will be invaluable in the rest of your degree as well as your future career. This is not just about honing your skills in quickly finding the information you need, but also how to resolve problems and debug issues with code yourself. 

### Finding Your Own Answers: Some Tips 

1. **Check the lecture slides**. Seems obvious. But you'd be surprised how many questions we get that are answered by a lecture slide that covered what you wanted to know. There may be a slide or an example that you missed that already explains something you wanted to know about or demonstrates some code similar to what you want to do. Look there first!

2. **Check this FAQ**. To save time reading through the entire FAQ, use the "Find" feature in your browser to search for certain words appearing on the page to do with your query (e.g. "Git", "Capybara", etc.) The "Find" feature is normally a menu item in the "Edit" menu.

3. **Check the discussion forums on Blackboard** to see if your question has already been answered. If it hasn't, don't post your own question just yet. There are more steps to try first.

4. **Check the docs**. Your question may be answered by the documentation for
   [Sinatra](http://sinatrarb.com/documentation.html),
   [SQLite](https://www.sqlite.org/docs.html) (see also [SQLite's SQL docs](https://www.sqlite.org/lang.html)),
   [Sequel](https://sequel.jeremyevans.net/documentation.html) (see also [Sequel's GitHub page](https://github.com/jeremyevans/sequel), which has lots of handy examples), 
   [RSpec](https://relishapp.com/rspec), and
   [Capybara](https://rubydoc.info/github/teamcapybara/capybara/master) (see also the handy [cheat sheet](https://devhints.io/capybara)).

5. **Use Google**. If you're unsure how to go about googling technical issues, or want to be more effective at using Google to find answers to programming questions, watch this video – "[Art of Googling as a Programmer](https://www.youtube.com/watch?v=JIV7wuihew8)" – for some tips. It's a bit Python-centric, but the principles apply to any programming language on any platform – and pretty much anything technical.

**If all of the above fails, you can ask a question.** See the next section on how to go about doing this.

### How Do I Go About Asking Questions?

To ensure you get a timely answer that resolves your problem, ensure you follow these steps:

* **For specific technical questions about your team project**, ask your demonstrator.

  <!--
  You can ask in the lab, or via Slack if the issue arises between
  labs and cannot wait until the next one. Bear in mind that your demonstrators
  are students too. They have assignments and deadlines of their own, so they
  may not respond immediately.
  -->

* **If your demonstrator cannot help you**, post a question in the appropriate forum in the [Coding Questions Discussion Board]([https://vle.shef.ac.uk/webapps/discussionboard/do/conference?toggle_mode=edit&action=list_forums&course_id=_107947_1&nav=discussion_board_entry&mode=cpview](https://vle.shef.ac.uk/webapps/discussionboard/do/forum?action=list_threads&course_id=_107947_1&nav=discussion_board_entry&conf_id=_346815_1&forum_id=_343693_1)) on Blackboard. 
  
  However, *don't post large chunks of your project's code in the forum*. If your problem only involves one or two lines of code that aren't important, that is fine; or, you might be able to obfuscate the code to demonstrate the same problem, but without using code directly lifted from your project.
  
  If your problem involves large segments or involves the whole project, then leave your team number and ensure you've pushed everything to the main branch of your repository (along with a detailed explanation of the problem you're experiencing). We can then clone your code and try to replicate the issue ourselves. 

* **Please don't email staff about technical issues directly.** Although we make our email addresses available, they're only to be used as a *last resort*. It is highly unlikely that you won't get a response using one of the methods above.

Naturally, when asking a question, help us to help you by including as much relevant information as possible. Screen shots are fine, but don't just post these without any context. If you don't provide all the information needed, we won't be able to resolve the issue.

## 2. Problems Running Code 

### When I try to run `sinatra` I get a `sinatra: command not found` message at the terminal, and my code refuses to run.

It would seem that you haven't set your Codio project up in the correct way – the way specified in the [Getting Started Instructions](./getting-started/README.md).

Note that you have to do this for every Codio project/box that you intend to run Sinatra projects with, including development and demonstration of your project.

### When I try to run one of the examples from the lectures found in this repository, it crashes with an error.

This is likely because you need to install the gems for the example first. In the terminal, ensure you have changed directory to the one containing the example, and type the following:

```
bundle install
```

The gems installed are the ones listed in the `Gemfile` in that directory. (Open the file to view what gems these are.)

You may need to refresh your memory on gems and Gemfiles. If so, go back to the material from the Autumn Semester (in particular, see Unit 7: Ruby Gems). You can also try Google of course for more information.

### When I run my web application or an example, Codio displays a "401 Authorization Required" message instead of the proper web page.

This is because Codio doesn't think you're logged into Codio on the web browser you're trying to use. 

First, open a tab and check you are indeed logged in. If you are, try clearing out your cookies in your browser settings, close and re-open your browser, log into Codio and try again. 

Sometimes Codio's cookies, which track whether a user is logged in or not, are blocked by a browser's default privacy mechanisms. Here are my experiences (and remedies) with certain browsers. Note that these are for Mac – your experience may differ!

* **Brave** – doesn't work. Remedy: Go to your browser settings, and select "Privacy & Security". Then go to "Cookies and other site data". Under "Sites that can always use cookies", add `codio.com` and `codio.io` separately. Ensure the "Including third-party cookies on this site" checkbox is selected.  Now close and re-open your browser, and log back into Codio. 
* **Chrome** – works fine.
* **Edge** – works fine. 
* **Firefox** – doesn't work. Remedy: Go to your browser settings, and select "Privacy & Security". Under "Enhanced Tracking Protection" click the "Manage Exceptions" button. Add `codio.com` and `codio.io`. Click "Save Changes". Now close and re-open your browser, and log back into Codio. 
* **Safari** – works fine.

Another reasons can be ad-blocking plugins that have been installed by you, the user. Try disabling these or making exceptions for the sites `codio.com` and `codio.io`. 

If the issue persists, try using another browser for your Codio work (e.g., one in the list above that works). This is usually enough to resolve the issue – I've never found this issue to be a machine-specific problem. 

### When I run my web application or an example, Codio displays a "502 Bad Gateway" error instead of the proper web page.

This is likely because you're not using the `sinatra` command to run your code and using the `ruby` command instead. Make sure you're using the `sinatra` command.

### I can't see the changes I made to my Sinatra application.

You have to stop (go to the terminal window and press "control" and "c") and then restart the web server (triggered by the `sinatra` command you used to start your application) each time you change any Ruby code in it (an exception is `.erb` files, changes for which can be seen without stopping and restarting).

This is a tedious thing to have to keep doing during development! So I recommend using `rerun`, as demonstrated in lectures. 

To do this prefix the `sinatra` command with `rerun`, for example as follows:

```
rerun sinatra hello_world
```

The rerun facility will keep checking for changes to your Ruby files and reload them when you make changes, meaning that you do not have to keep stopping and restarting the web server each time you make a change to your project.

Note that you don't need to restart the web server if you only made changes to view files. 


### I can't see the changes I made to my CSS / my CSS is not updating. 

Ensure that your browser is not caching your CSS files (i.e., using a stored, out of date copy, rather than a fresh version from your web application).

Clear out your browser cache, or switch off caching altogether. Google how to do this for the browser you're using.

### Our team project works for my teammates but crashes with an error on my Codio box.

These kinds of issues ("it works for my teammates but not for me") are almost always (99% of the time) to do with differences in the gems that are installed on different Codio boxes. If you think about it logically, what else could be the difference in setup between your Codio box and theirs, since each box is practically identical in terms of its configuration at the beginning. (When trying to debug, try to think about differences between "when it works" and "when it doesn't".)

If you issue a `gem list` command at the terminal, you will be able to see a list of gems installed on your box, and you can compare it with that of your teammates'. (The list can be quite long!)

You can also use the `reset_gems` command to reset the gems installed on your box.

Make sure that your project has all the gems it needs by keeping your `Gemfile` up to date. This is the key to avoiding these kinds of problems in the first place. 

### I'm getting an error message `cannot load such file -- sequel (LoadError)`. I have the sequel gem installed, so I'm confused as to what is going on.

You need the `sqlite3` gem installed as well. Make sure both the `sequel` and the `sqlite3` gems are part of your project's `Gemfile`.

### What are the gems we will need for the team project?

Depending on how far through the lectures we are, we may not have encountered all of these, so don't worry about the ones you don't recognise (yet):

* **Core gems** include `sinatra`, `puma` (the web server), `rerun` (which gives you the ability to restart the webserver when you change your code, so that you do not have to do it manually), `require_all` (for automatically "requiring" all Ruby files in a directory), `rubocop` (for coding standards and style checking). 

* For the **database**, you'll need at least `sequel` and `sqlite3`. Don't forget the `sqlite3` gem, otherwise you'll get some confusing error messages.  

* For **encrypting user data** (i.e., to preserve data confidentiality), you'll need `openssl`.

* For **code style checking**, you'll need `rubocop`. To extend style checking to RSpec and Sequel code, you'll also need `rubocop-rspec` and `rubocop-sequel` respectively.

* For **testing**, you'll need at least `capybara` (for acceptance tests), `simplecov` (for coverage tracking), `rackup`, and `rspec`.

Note that some of these gems may already be installed on a fresh Codio box. In general, it's good practice to include them in your Gemfile regardless for development/deployment environments where they aren't.

### When testing, my application seems to behave differently compared to when it's being used for real. 

This is often to do with differences between the "test" database and the "development" database. If certain data is not present in the test database, the application may behave differently. If you're experiencing some differing behaviour, the first thing you can check is the log files produced by Sequel. Check the queries are the same when the application is being run in "production" mode compared to when it is being tested.

## 3. Problems with Git

### I cannot clone my team's repository.

GitLab uses SSH keys to authenticate you rather than passwords. If you're getting errors or are being asked for your password when you try to clone your team's repository, it's probably because you did not set up GitLab with your Codio SSH keys last semester. That is, you didn't complete both parts of Unit 8, which is about Git. I'd strongly recommend you go back and do both of these units, because Git is very important this semester.

To set up your SSH keys, sign into Codio, then click your username in the bottom left profile. Under "My Account", there should be a menu item called "SSH Keys". If you click this link, you'll be taken to a page with a grey box at the top, with your public SSH key in it. Ensure that you select and copy the entire contents of this box (and *only* the contents of the box). Now, log into GitLab (https://git.shefcompsci.org). Click the icon in the top right of the page to reveal a drop-down box, and select "Preferences". Select "SSH Keys" from the sidebar that appears. In the big text box that appears, paste your SSH key. In the title box, enter "Codio". Then click the "Add key" button.

Other possible reasons:

* Your team number is 1-9 and you're not using a zero before your team number in the `git clone` commmand. Your repository uses two digit team numbers, so `01`, `02`, etc.

* You're trying to clone another team's repository. Check your team number!

* There's been an administrative error, and you don't have the necessary permissions to clone your team's repository. This is the most unlikeliest of the possibilities, so check you have done all of the above first. However, it does happen from time to time, so if you're still experiencing problems, this is one of the few occasions where you can [send me – Phil McMinn – an email](mailto:p.mcminn@sheffield.ac.uk). Make sure that you include your Sheffield computer account username in the body of the email.

## 4. Using Codio

### I don't really like Codio. Can I use my own machine to develop on instead?

Codio provides a standardised environment to students that removes many issues related to incompatibilities between different operating systems and setups.

This is to your benefit – firstly, you won't have to debug these kinds of issues across the various machine setups your team members may have, and secondly, because Codio makes it easy for *us to help you* if you encounter problems with your code. 

It's not impossible though to develop everything on your own machine. However, this means you installing Ruby and getting everything working yourself. We are unable to provide support for students' individual machines, since fixing individual machine setups is very time consuming and our priority is helping with programming questions and issues.  

Furthermore, since the team project will be marked using Codio, everything needs to work on Codio, because the markers will not be debugging your code to get it to run. This means that if you use your own machine, you will need to get the same versions of Ruby, SQLite, and all the gems that you're using, ensuring all behaviours are identical across different machines. 

### I've heard it's possible to use VSCode on Codio. Is that true?

Yes! See the [final section in the Getting Started instructions](getting-started/README.md#using-vscode).

