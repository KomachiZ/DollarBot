# 💰 Dollar Bot 💰

<!-- TABLE OF CONTENTS -->
<b><h3>Table of Contents</h3></b>
  <ol>
    <li><a href="#whats-dollarbot">What's DollarBot?
    <li><a href="#why-use-dollarbot">Why use DollarBot?</a></li>
<!--     <li><a href="#check-out-the-video">Check out the video!</a></li> -->
    <li><a href="#whats-new">What's new in this version?</a></li>
    <li><a href="#installation-and-setup">Installation and Setup</a></li>
   <li><a href="#functionalities">Functionalities</a></li>
   <li><a href="#contributors">Contributors</a></li>
   <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>

Are you a developer? <a href="https://github.com/aditikilledar/dollar_bot_SE23/blob/main/Developer_ReadMe.md">Click here: For Developers and Future Contributors</a>

[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/usmanwardag/auto_anki)

![MIT license](https://img.shields.io/badge/License-MIT-green.svg)
[![Platform](https://img.shields.io/badge/Platform-Telegram-blue)](https://desktop.telegram.org/)
![GitHub](https://img.shields.io/badge/Language-Python-blue.svg)
[![GitHub contributors](https://img.shields.io/github/contributors/sak007/MyDollarBot-BOTGo)](https://github.com/sak007/MyDollarBot-BOTGo/graphs/contributors)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5759217.svg)](https://doi.org/10.5281/zenodo.5759217)
[![Build Status](https://app.travis-ci.com/usmanwardag/dollar_bot.svg?branch=main)](https://app.travis-ci.com/usmanwardag/dollar_bot)
[![codecov](https://codecov.io/gh/usmanwardag/dollar_bot/branch/main/graph/badge.svg?token=PYAWX95R67)](https://codecov.io/gh/usmanwardag/dollar_bot)

[![GitHub issues](https://img.shields.io/github/issues/sak007/MyDollarBot-BOTGo)](https://github.com/sak007/MyDollarBot-BOTGo/issues?q=is%3Aopen+is%3Aissue)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/sak007/MyDollarBot-BOTGo)](https://github.com/sak007/MyDollarBot-BOTGo/issues?q=is%3Aissue+is%3Aclosed)

<hr>

## What's DollarBot?

DollarBot is a handy little bot built on top of Telegram, to help you with daily expense tracking and analytics on your past spends. 

It's easy to setup, run and use on a daily basis!

## Why use DollarBot?

With simple in-chat commands, this bot helps you:
- Add/Record new spendings
- Display your spendings through engaging graphs
- Show the sum of your expenditure for the current day/month
- Display your spending history
- Clear/Erase all your records
- Edit/Change any spending details if you wish to
- View Analytics and export as csv

## Check out the video!

[![Demo Video](https://i9.ytimg.com/vi/aCjcT1CHAzU/mq3.jpg?sqp=COSotI0G&rs=AOn4CLD34jFIlq6GRdmTnK6p3F8O2F-Yig)](https://youtu.be/aCjcT1CHAzU)

## What's new?

We've considerably extended this project to make using DollarBot easy and engaging.
1. Clearer wording in the documentation.
2. Expressive Graphs
3. Budget Creation Updated
4. Analytics
5. Clearer PDF Reports
6. CSV Reports for Analytics use

Check [this documentation out](https://github.com/aditikilledar/dollar_bot_SE23/blob/main/docs/Whats_new.pdf) for an in-depth depiction of our changes. :)

## Installation and Setup

### Pre-requisite: The Telegram Desktop App

Since DollarBot is built on top of Telegram, you'll first need:
1. Download the Telegram Desktop Application <a href="https://desktop.telegram.org/">here.</a>
```https://desktop.telegram.org/```
2. Create a Telegram account or Sign in.

Open up your terminal and let's get started:

### MacOS / Ubuntu Users

1. Clone this repository to your local system. 
```
   git clone https://github.com/aditikilledar/dollar_bot_SE23/
```
2. Start a terminal session in the directory where the project has been cloned. Run the following commands and follow the instructions on-screen to complete the installation.
```
  chmod a+x setup.sh
  bash setup.sh
```
There, all done!

The installation is easy for MacOS or on UNIX terminals. 

### Windows

With Windows, you'll need to use a platform to execute UNIX-like commands in order to execute the setup.sh bash script. Once in the platform, use the steps in the MacOS/Unix Section above to setup DollarBot.

We've used <a href="https://www.cygwin.com/">Cygwin,</a> but there are more options like WSL that you can explore.

Additionally, find more hints on Cygwin installation <a href="https://stackoverflow.com/questions/6413377/is-there-a-way-to-run-bash-scripts-on-windows">here.</a>

## Running DollarBot:

Once you've executed setup.sh, and all dependencies have been installed, you can start running DollarBot by following these instructions.

1. Open the Telegram Desktop Application and sign in. Once inside Telegram, search for "BotFather". Click on "Start", and enter the following command:
```
  /newbot
```
2. Follow the instructions on screen and choose a name for your bot (e.g., `dollarbot`). After this, select a UNIQUE username for your bot that ends with "bot", for example: `dollarbot_<your_nickname>`.

3. BotFather will now confirm the creation of your bot and provide a TOKEN to access the HTTP API - copy and save this token for future use. Make sure you save this token– don't lose it!

4. In the repo directory (where you cloned it), run these commands.

(a) grant execution access to a bash script
  ```
  chmod a+x run.sh
  ```

(b) execute the run.sh bash script to start DollarBot
   
###### MacOS / Unix
```
   bash run.sh
```
###### Windows
```
   ./run.sh
```

```Note```: It will ask you to paste the API token you received from Telegram while creating your bot (Step 3), so keep that handy.
A successful run will generate a message on your terminal that says "TeleBot: Started polling." 

5. In the Telegram app, search for your newly created bot by entering your UNIQUE username and open the bot you created.

6. Now, on Telegram, enter the "/start" or "menu" command, and you are all set to track your expenses!

### Run Automatically at Startup

To run the script automatically at startup / reboot, simply add the `.run_forever.sh` script to your `.bashrc` file, which executes whenever you reboot your system.
<a href="https://stackoverflow.com/questions/49083789/how-to-add-new-line-in-bashrc-file-in-ubuntu">Click here for help adding to .bashrc files.</a>

## Functionalities

Here's a quick overview of how each of the commands work. Also see: Link at the end of each example for a more detailed version of the documentation.

### Add

``` add example add code here ``` 
[insert a GIF showing how to run here]

[Learn more here](https://github.com/aditikilledar/dollar_bot_SE23/blob/docu-merging-scattered-docs/docs/add.md)

### Budget

#### Delete

#### Update

#### View

### Delete

### Edit

### Estimate

### Graphing and Analytics

Use /analytics to gain graphical insights about your budgets and spending.

[Learn more here](https://github.com/aditikilledar/dollar_bot_SE23/blob/main/docs/analytics.md)

### Helper

### History


## Contributors
<table>
  <tr>
    <td align="center"><a href="https://github.com/aditikilledar"><img src="https://avatars.githubusercontent.com/u/73051765?v=4" width="75px;" alt=""/><br /><sub><b>Aditi Killedar</b></sub></a></td>
    <td align="center"><a href="https://github.com/shashank-madan"><img src="https://avatars.githubusercontent.com/u/52149707?s=80&v=4" width="75px;" alt=""/><br /><sub><b>Shashank Madan</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/srina1h"><img src="https://avatars.githubusercontent.com/u/47570142?v=4" width="75px;" alt=""/><br /><sub><b> Srinath Srinivasan</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/aiyer786"><img src="https://avatars.githubusercontent.com/u/52149707?s=80&v=4" width="75px;" alt=""/><br /><sub><b>Aditya Iyer</b></sub></a><br /></td>
  </tr>
</table>

## Acknowledgements

- We would like to express our gratitude 🙏🏻 and a big thank you 😇 to Prof. Dr. Timothy Menzie for giving us the opportunity to get into the shoes of software building and learning new skills and development process throught the project building.
- A big thank you 😊 to the Teaching Assistants for their support.
- Thank you to the previous team 😊 for a thorough ReadMe and deatiled documentation.[MyDollarBot](https://github.com/sak007/MyDollarBot-BOTGo)
- Thank you to the ⭐️[Telegram bot](https://github.com/python-telegram-bot/python-telegram-bot)




