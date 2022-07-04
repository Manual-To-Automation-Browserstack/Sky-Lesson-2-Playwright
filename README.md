![Logo](https://www.browserstack.com/images/static/header-logo.jpg)

# Manual To Automation @ SKY - Lesson 2 in Playwright <a href="https://nodejs.org/en/"><img src="https://raw.githubusercontent.com/github/explore/60cd2530141f67f07a947fa2d310c482e287e387/topics/playwright/playwright.png" alt="playwright" height="22" /></a>

## Introduction

This code provides the solution to the exam given at the end of the second lesson in the Manual To Automation @ SKY training series. It is a simple Playwright application that opens a web page, opens the search hover, and performs a search.

The trick to this solution is in figuring out how to navigate the contents of the iFrame that contains the consent box that appears on the page. Users need to research how to switch to these iFrames in order to find the elements contained within. They also need to figure out how to move back to the main HTML body after that interaction.

---

## Installation

There are a few things that you will need before you can get started.

* NodeJS - use [this](https://phoenixnap.com/kb/install-node-js-npm-on-windows) guide for Windows and [this](https://nodesource.com/blog/installing-nodejs-tutorial-mac-os-x/) guide for Mac.
* Git for pulling down the code - follow [this]() guide for installing Git on all platforms. There are other useful guides on the website mentioned previously. Start [here](https://github.com/git-guides) anad follow through to the various links to learn more about Git. It will be very useful on your automation journey. If you have any issues with tokens or user credentials, let me know as this can trip a lot of people up.
* Visual Studio Code - You can download VS Code for free from [here](https://code.visualstudio.com/download). This is a very useful tool for writing and running your code as it has auto complete, and powerful debugging capabilities. [This](https://code.visualstudio.com/docs/introvideos/basics) is a handy starting point for how to get started with VS Code.

Once you have these installed, you are good to go to the next step.

Follow the below steps to get the code onto your local machine.

* Open a terminal. (Terminal on Mac, Command Prompt on Windows)
* Go to the directory where you want to place the code using [cd](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/cd) for Windows, and it functions mostly the same for Mac. You just use "cd" but the folder structure on Mac is different (/Users/username/Documents instead of C:/Users/username/Documents)
* Copy the following command into the terminal, (remember, you must have [Git](https://git-scm.com/downloads) installed)
```sh
git clone https://github.com/Manual-To-Automation-Browserstack/Sky-Lesson-2-Playwright.git.
```
* Move into the directory that you just cloned by typing
```sh
cd Sky-Lesson-2-Playwright
```
* When inside this directory, copy the following command and run it:
```sh
npm install
```
* Once all the dependencies are installed, you will be able to run the tests by using the following commands:
```sh
# Runs the first.spec.js file
npm run first-test

# Runs all of the files in the tests directory
npm run all

# Run all the tests while opening the browser locally (useful to see everything happening in real time.)
npm run headed
```

These scripts are useful to get started. You can add more as needed in the "scripts" section of the [package.json](./package.json) file. Once you have added one, you then simply run:

```sh
npm run <insert script name>
```

For a full list of the various command line options for running Plawright tests, see [this](https://playwright.dev/docs/test-cli) link.
