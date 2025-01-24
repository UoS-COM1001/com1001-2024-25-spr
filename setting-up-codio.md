# Setting Up Codio

**NOTE:** you can watch me go through the contents of this README in a video on [Blackboard]().

### Contents of this README file

1. [Logging into Codio](#1-logging-into-codio)
2. [Creating a Project](#2-creating-up-a-project)
3. [Hello, World!](#3-hello-world)
4. [Cloning the Examples Repository on Codio](#4-cloning-the-examples-repository-on-codio)
5. [Cloning your Team's Repository](#5-cloning-your-teams-repository)
6. [Using VSCode](#6-using-vscode)

## 1. Logging into Codio

In the last semester, you exclusively accessed Codio through the units, but this semester it's easier to sign into Codio directly, which means you'll need a password. Go to https://codio.com and click the "Sign In" link. If you don't already have a password, click the "Lost your password?" link and enter your university email address (ok, so you didn't lose it, you never had one in the first place — but this is how to get one!). Ensure you set your password to something secure and hard for others to guess.

## 2. Creating a Project

You'll then need to set up your own virtual machine on Codio. You'll be using this to develop on and run the examples from the lectures. With Codio, you set up a virtual machine - usually called a "Codio box", or just a "box" - by configuring something called a project.

To do this, sign in, and click the  **"My Projects"** link under the "BUILD" in the left sidebar, and click the **"New Project"** button at the top of the page.

Under **"Choose your Starting Point"** you need to select "Sinatra". However, the option won't be there the first time you do this. You will need to click "+browse for more". In the search box type "sinatra" and press enter. You should then see a button that says "THE UNIVERSITY OF SHEFFIELD/SINATRA", with a hat logo. Ensure this is selected.

Give your project a name under **"Add some details"**. You can call your project anything you like – but if you have more than one project, you'll need to ensure they each have a unique name.  Ensure **"Select the visibility"** is "Private".

**You're now ready to create your box by clicking "Create".**

A few seconds may elapse, but then you'll see a screen saying "Loading Project...", followed by a new screen. This is now your project. When you next sign into Codio, you can just go to "My Projects", and your project will be listed with the name you chose. You can just click it to restart it - you don't need to create a new project each time you sign in.

## 3. Hello, World!

We're now going to create a quick and simple Sinatra application.

First open a new terminal (it's the first option under "Tools" menu, or the middle icon under your project name in the left sidebar). Create a new directory called `hello_world` using the `mkdir` command, and then change the current directory the terminal is in to it, using the `cd` command.

```console
mkdir hello_world
cd hello_world
```

You should see a folder called `hello_world` in the file tree in the left sidebar of the Codio interface. However it's empty, so you cannot reveal any files in it. You can confirm this by typing

```console
ls -al
```

which should report a total of 0 files and directories.

Now, we're going to create our first Sinatra application. Type:

```console
create_app
```

An arrow should appear next to the `hello_world` directory in the file tree, and clicking on it should reveal a series of entries. You can confirm this in the terminal by typing `ls -al` again.

One of the subdirectories in the filetree is called `controllers`. Right-click on controllers and select "New File...". In the dialog box that appears, enter `hello_world.rb` as the filename. In the file editor that now opens, enter the following code:

```ruby
get "/hello-world" do
  "Hello, World!"
end
```

You can now run this application by going back to the terminal and typing:

```console
sinatra
```

This command will start a web server that is serving your application. If you did everything correctly, then as part of the blurb outputted by the command will be a yellow link that starts with `https:// ...` and ends with `-4567.codio.io/hello-world`. Clicking this link opens a new browser window that "runs" the code you just wrote and outputs the message "Hello, World!".

An alternative way to start the web server is to click the "Run" button that is next to the menu bar. This works so long as you are currently editing a file somewhere in your application. You can also use the "View" button instead of clicking the yellow link, but make sure that in the dropdown "New Browser Tab" is selected as the "Inside Codio" option does not work. 

When you have finished your session, type control and "C" together to exit Sinatra. (After you've exited, don't expect to see any more pages served at the URL until you restart Sinatra again.)

## 4. Cloning the Examples Repository on Codio

In addition to this GitHub repository there is another that contains a series of Sinatra code examples that will be discussed in lectures. You can clone this repository by opening a terminal and entering the following command:

```console
git clone https://github.com/UoS-COM1001/com1001-examples.git
```

You don't need to understand these now, but feel free to take a look at them and run them. Occasionally these will be updated and/or bugs will be fixed, so do a `git pull` regularly.

## 5. Cloning Your Team's Repository

While the course materials are all on GitHub, your team's repository can be found on GitLab.

Your team's repository may be found on GitLab. To clone it, make sure you're somewhere appropriate in your filetree in the Terminal. The best place is probably the `workspace` directory. The `workspace` directory is the directory the Terminal opens in, where all subdirectories and files are listed in the left sidebar. So if you've followed all the instructions correctly so far, your sidebar should have just the `hello-world` directory and the `com1001-examples` repository directory listed in it.

To clone your team's repository, you'll need to run the command:

```console
git clone git@git.shefcompsci.org.uk:com1001-2024-25/teamXX/project.git
```

replacing `XX` in the command with your two-digit team number (if you're in team 1-9, you'll need to enter a leading zero, i.e., 01, 02 etc.) Again, type "yes" to any authenticity questions.

This will create a directory called `project`, which is where the Sinatra application will live that your team will build. If `project` is an empty directory (i.e., a team mate of yours did not already get to these instructions first) you may run `create_app` in it. Be sure your terminal is actually "in" the `project` directory before you do this, so that you don't create an application in the wrong place. You can then commit and push these files back to the repository.

Check you can commit, push, and pull files to and from the repository correctly using the appropriate commands.

If you are experiencing problems with this step, check out the technical FAQ &mdash; [I cannot clone my team's repository](./technical-FAQ.md#i-cannot-clone-my-teams-repository).

## 6. Using VSCode

The standard text editor in Codio is rather basic, but you can used Visual Studio Code [(VSCode)](https://code.visualstudio.com) instead. VSCode is a popular text editor and IDE for many languages, and may be used in a web browser on Codio itself. Assuming you have followed in the previous instructions in the first lecture and have everything setup in Codio, then you will have a Codio box already up and running. In Codio, go to "Tools", then "Install Software". Scroll down the list and select "VSCode". VSCode will be now available at a special URL in your web browser for use with your Codio files. The URL you need to access it depends on your Codio box name. This is different from your project's name. Your Codio box name is the subdomain of your Codio Box domain, which Codio tells you in the prompt of every Terminal session that you start. For example, my Terminal prompt is the following:

```console
codio@everton-fan:~/workspace$
```

This means my box name is ``everton-fan``. This means the URL I would be accessing VSCode from, if I installed it, would be https://everton-fan-4000.codio.io. Note that this URL is essentially the same as the Base URL of your web applications launched from Codio (something we will discuss in week 1's lectures), but using port 4000.


