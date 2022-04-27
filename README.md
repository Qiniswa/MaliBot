# MaliBot
<p align="center">
A bot that helps you excel on your daily tasks. 
<p align="center">
MaliBot is a Telegram bot created through the Telegram API. It is designed to track and help with your daily sessions. It uses Node's Natural Language Processing to distinguish phrases and categorize them into specified intents, in order to provide a suitable response. It has built-in methods (such as "/pomodoro") that allow users to utilize their functions. 
  
  
## At a Glance

  
  ## Current Methods
  ### 1. The Pomodoro Technique
  
>The Pomodoro Technique is a time management method developed by Francesco Cirillo in the late 1980s. The technique uses a timer to break down work into intervals traditionally 25 minutes in length, separated by short breaks. These intervals are known as "pomodori", from the Italian word pomodoro for "tomato". The method is based on the idea that frequent breaks can improve mental agility.

After you have entered "/pomodoro \<session name\>", \<session name\> executes.

- Sending the text `/pomodoro status` will let you know how much time you have left in your current Pomodoro session or break.
- Sending any other phrase will start a 30 minute pomodoro session. You'll be notified 30 minutes later via text to take a break. And then will be notified 7 minutes after that to get back to work (at which point you can send another phrase to start the Pomodoro session).
- Sending the word `/pomodoro clear` will clear all sessions. 

<b> Example conversation: </b>
- `/pomodoro status`: "No pomodoro session is currently running."
- `/pomodoro Physics Lab`: "Session "Information Systems class" started on 11/02/2021, 11:00:00 AM."
- `/pomodoro status`: "Session "Information Systems class" is currently running. You have 30 minute(s) left."
- Work for 30 minutes....
- You'll get a text: ""30 minutes done! Take a break.""
- `/pomodoro status`: "You're on break from "Information Systems class"! You have 7 minute(s) left before work."
- Do something for 7 minutes to your heart's content...
- You'll get a text: "7 minutes done. Back to work!"
- `/pomodoro status`: "No pomodoro session is currently running."
- And so on...

## Get Started
Get your own Telegram token from BotFather. More on that [here](https://core.telegram.org/bots). Then, plug in the token at the top of index.js.

1. Clone this reposity and run:
```sh
npm install
```
2. Run the bot:
```sh
npm run bot
```
