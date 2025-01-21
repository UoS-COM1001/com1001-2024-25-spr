# Getting Started

**NOTE:** you can watch me go through the contents of this README in a video on [Blackboard]().

### Contents of this README file

1. [Setting up Codio](#1-setting-up-codio)
2. [Cloning this Repository on Codio](#2-cloning-this-repository-on-codio)
3. [Running an Example](#3-running-an-example)

## 1. Setting up Codio

### Obtaining a Password

In the last semester, you may have exclusively accessed Codio through the units, but this semester you'll need to sign into Codio directly, which means you'll need a password. Go to https://codio.com and click the "Sign In" link. If you don't already have a
password, click the "Lost your password?" link and enter your university email address (ok, so you didn't lose it, you never had one in the first place — but this is how to get one!).

### Setting up a Project

You'll then need to set up your own virtual machine on Codio. You'll be using this to develop on and run the examples from the lectures. With Codio, you set up a virtual machine - usually called a "Codio box", or just a "box" - by configuring something called a project. 

To do this, sign in, and click the  **"My Projects"** link under the "BUILD" in the left sidebar, and click the **"New Project"** button at the top of the page. 

Under **"Choose your Starting Point"** you need to select "Sinatra". However, the option won't be there the first time you do this. You will need to click "+browse for more". In the search box type "sinatra" and press enter. You should then see a button that says "THE UNIVERSITY OF SHEFFIELD/SINATRA", with a hat logo. Ensure this is selected. 

Give your project a name under **"Add some details"**. You can call your project anything you like – but if you have more than one project, you'll need to ensure they each have a unique name.  Ensure **"Select the visibility"** is "Private".

**You're now ready to create your box by clicking "Create".**

A few seconds may elapse, but then you'll see a screen saying "Loading Project...", followed by a new screen. This is now your project. When you next sign into Codio, you can just go to "My Projects", and your project will be listed with the name you chose. You can just click it to restart it - you don't need to create a new project each time you sign in. 

## 2. Cloning this Repository on Codio

Open a terminal in your project (it's the first option under "Tools" menu, or the middle icon under your project name in the left sidebar), and enter the following command:

```console
git clone https://github.com/UoS-COM1001/com1001-2024.git
```

(If you hover over the command, a clipboard icon will appear. If you click it, you can copy the command to your clipboard and then paste it into your terminal.)

You'll be asked a question ("Are you sure you want to continue connecting ... ?") - just type "yes", followed by enter.

## 3. Running an Example

To run an example you'll need to change to the directory where it exists as a Ruby file. You'll need to ensure the appropriate gems are installed. Each directory contains a `Gemfile` so it is easy for you to ensure this using [Bundler](https://bundler.io). Bundler is already installed on Codio, so you just need to issue a `bundle install` command in the terminal in the appropriate directory. 

To run an example, you will need to change to the directory of the example and then use the `sinatra` command, followed by the filename.

For example, to run the `hello_world.rb` example in the ``getting-started``
directory, you would need to open a Terminal and enter the following commands:

1) Change to the appropriate directory using the `cd` command:

```console
cd com1001-2024/getting-started/
```

If you type `ls` in this directory, you'll see there is one example called `hello_world_example`, so then type:

```console
cd hello_world_example
```

If you type `ls` now, you should see three files, one of which is called `hello_world.rb`, which is the Sinatra example we want to run. 

2) Run the `sinatra` command:

Type:

```console
sinatra hello_world.rb
```

Most examples are full applications with an `app.rb` file. To run these you can just run the `sinatra` command without any arguments in the directory containing `app.rb`.

Not all `.rb` files in a directory can be run, since they are a component part of an overall application, and not an "entry point" designed to be run themselves. It should be clear from the explanations in lectures and looking at the code itself which files are meant to be run and which ones are not.

## 4. Cloning Your Team's Repository

Your team's repository may be found on GitLab. To clone it, make sure you're somewhere appropriate in your filetree in the Terminal. The best place is probably the `workspace` directory. The `workspace` directory is the directory the Terminal opens in, where all subdirectories and files are listed in the left sidebar. So if you've followed all the instructions correctly so far, your sidebar should have the COM1001 repository directory listed in it – `com1001-2024`.

To clone your team's repository, you'll need to run the command:

```console
git clone git@git.shefcompsci.org.uk:com1001-2023-24/teamXX/project.git
```

replacing `XX` in the command with your two-digit team number (if you're in team 1-9, you'll need to enter a leading zero, i.e., 01, 02 etc.) Again, type "yes" to any authenticity questions. 

Check you can commit, push, and pull files to and from the repository using the appropriate commands.

If you are experiencing problems with your team's repository let Phil McMinn or your demonstrator know immediately. BUT BEFORE YOU DO THIS, NOTE: If you haven't yet completed the Revision Control (week 8) units from last semester as to how to use Git, make sure you've done them before you contact us (or, if think you might need a refresher). In particular, you will need to set GitLab up with your personal Codio SSH keys as described in the second unit. If you haven't completed this step, you will not be able to clone your team's GitLab repository for completing the project. 

## 5. Advanced Codio

### Using VSCode

The standard text editor in Codio is rather basic, but you can used Visual Studio Code [(VSCode)](https://code.visualstudio.com) instead. VSCode is a popular text editor and IDE for many languages, and may be used in a web browser on Codio itself. Assuming you have followed in the previous instructions in the first lecture and have everything setup in Codio, then you will have a Codio box already up and running. In Codio, go to "Tools", then "Install Software". Scroll down the list and select "VSCode". VSCode will be now available at a special URL in your web browser for use with your Codio files. The URL you need to access it depends on your Codio box name. This is different from your project's name. Your Codio box name is the subdomain of your Codio Box domain, which Codio tells you in the preamble of every Terminal session that you start. For example, my Terminal session prints out the following:

```
 *
 * Welcome to the Codio Terminal!
 *
 * https://docs.codio.com/project/ide/boxes/#overview
 *
 * Your Codio Box domain is: everton-fan.codio.io
 *
```

This means my box name is ``everton-fan``. This means the URL I would be accessing VSCode from, if I installed it, would be https://everton-fan-4000.codio.io. Note that this URL is essentially the same as the Base URL of your web applications launched from Codio (as discussed in lectures), but using port 4000.


