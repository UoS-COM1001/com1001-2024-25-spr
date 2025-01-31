# Getting Started

**NOTE:** you can watch me go through the steps of this README in a video on
[Blackboard]().

### Contents of this README file

1. [Logging into Codio](#1-logging-into-codio)
2. [Hello, World!](#3-hello-world)
3. [Cloning the Examples Repository on
   Codio](#4-cloning-the-examples-repository-on-codio)
4. [Cloning your Team's Repository](#5-cloning-your-teams-repository)
5. [Using VSCode](#6-using-vscode)

## 1. Logging into Codio

Go to [COM1001 on
Blackboard](https://vle.shef.ac.uk/ultra/courses/_116942_1/outline). Scroll down
to "Learning Materials: Semester 2", and reveal the contents. Then click "COM1001 
Spring Semester on Codio". 

This should load your personal "project" on Codio. This will be where you do
your coding on your team project, and run examples discussed in lectures and
write any code to try-out any principles outside of the team project itself.

## 2. Hello, World!

We're now going to create a quick and simple Sinatra application.

First open a new terminal (it's the first option under "Tools" menu, or the
middle icon under your project name in the left sidebar). Create a new directory
called `hello_world` using the `mkdir` command, and then change the current
directory the terminal is in to it, using the `cd` command.

```console
mkdir hello_world
cd hello_world
```

You should see a folder called `hello_world` in the file tree in the left
sidebar of the Codio interface. However it's empty, so you cannot reveal any
files in it. You can confirm this by typing

```console
ls -l
```

which should report a total of 0 files and directories.

Now, we're going to create our first Sinatra application. Type:

```console
create_app
```

An arrow should appear next to the `hello_world` directory in the file tree, and
clicking on it should reveal a series of entries. You can confirm this in the
terminal by typing `ls -al` again.

One of the subdirectories in the filetree is called `controllers`. Right-click
on controllers and select "New File...". In the dialog box that appears, enter
`hello_world.rb` as the filename. In the file editor that now opens, enter the
following code:

```ruby
get "/hello-world" do
  "Hello, World!"
end
```

You can now run this application by going back to the terminal and typing:

```console
sinatra
```

This command will start a web server that is serving your application. If you
did everything correctly, then as part of the blurb outputted by the command
will be a yellow link that starts with `https:// ...` and ends with
`-4567.codio.io/hello-world`. Clicking this link opens a new browser window that
"runs" the code you just wrote and outputs the message "Hello, World!".

An alternative way to start the web server is to click the "Run" button that is
next to the menu bar. This works so long as you are currently editing a file
somewhere in your application. You can also use the "View" button instead of
clicking the yellow link, but make sure that in the dropdown "New Browser Tab"
is selected as the "Inside Codio" option does not work.

When you have finished your session, press "control" and "c" together on your
keyboard to exit Sinatra. (After you've exited, don't expect to see any more
pages served at the URL until you restart Sinatra again.)

## 3. Cloning the Examples Repository on Codio

In addition to this GitHub repository there is another that contains a series of
Sinatra code examples that will be discussed in lectures. You can clone this
repository by opening a terminal and entering the following command:

```console
git clone https://github.com/UoS-COM1001/com1001-examples.git
```

You don't need to understand these now, but feel free to take a look at them and
run them. Occasionally these will be updated and/or bugs will be fixed, so do a
`git pull` regularly.

## 4. Cloning Your Team's Repository

While the course materials are all on GitHub, your team's repository can be
found on GitLab.

Your team's repository may be found on GitLab. To clone it, make sure you're
somewhere appropriate in your filetree in the Terminal. The best place is
probably the `workspace` directory. The `workspace` directory is the directory
the Terminal opens in, where all subdirectories and files are listed in the left
sidebar. So if you've followed all the instructions correctly so far, your
sidebar should have just the `hello-world` directory and the `com1001-examples`
repository directory listed in it.

To clone your team's repository, you'll need to run the command:

```console
git clone git@git.shefcompsci.org.uk:com1001-2024-25/teamXX/project.git
```

replacing `XX` in the command with your two-digit team number (if you're in team
1-9, you'll need to enter a leading zero, i.e., 01, 02 etc.) Again, type "yes"
to any authenticity questions.

This will create a directory called `project`, which is where the Sinatra
application will live that your team will build. If `project` is an empty
directory (i.e., a team mate of yours did not already get to these instructions
first) you may run `create_app` in it. Be sure your terminal is actually "in"
the `project` directory before you do this, so that you don't create an
application in the wrong place. You can then commit and push these files back to
the repository.

Check you can commit, push, and pull files to and from the repository correctly
using the appropriate commands.

If you are experiencing problems with this step, check out the technical FAQ
&mdash; [I cannot clone my team's
repository](./technical-FAQ.md#i-cannot-clone-my-teams-repository).

## 5. Using VSCode

The standard text editor in Codio is rather basic, but you can use Visual
Studio Code [(VSCode)](https://code.visualstudio.com) instead. VSCode is a
popular text editor and IDE for many languages and may be used in a web browser
on Codio itself. 

You can access VSCode using the button to the right of the "Run" button in the 
menu bar. It can operate within Codio itself, or in a completely separate 
browser tab (have a play with the drop-down options).
