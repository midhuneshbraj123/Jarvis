# Jarvis ⚡

A lightweight, 24/7 Slack bot built with Node.js and the Slack Bolt framework that responds to custom slash commands with latency checks, random cat facts, and jokes[cite: 3, 4].

## Features

* **`/jarvis-ping`** — Checks bot responsiveness and latency[cite: 3].
* **`/jarvis-help`** — Lists all available commands and their descriptions[cite: 3].
* **`/jarvis-catfact`** — Fetches and displays a random cat fact using the Cat Fact API[cite: 3].
* **`/jarvis-joke`** — Fetches and tells a random joke using the Official Joke API[cite: 3].

## Tech Stack

* **Runtime:** Node.js
* **Framework:** `@slack/bolt`
* **HTTP Client:** `axios`[cite: 2, 3]
* **Environment Management:** `dotenv`
* **Process Manager (Deployment):** PM2

  <img width="1916" height="977" alt="banner" src="https://github.com/user-attachments/assets/7c9f4f71-7790-4034-81ad-41aede293684" />

## Project Structure

```text
Jarvis/
└── my-slack-bot/
    ├── .env               # Secret Slack tokens (ignored by Git)[cite: 1]
    ├── .gitignore         # Specifies untracked files[cite: 1]
    ├── index.js           # Main bot application and command handlers[cite: 1, 3]
    ├── package.json       # Project metadata and dependencies[cite: 1]
    └── package-lock.json  # Dependency lockfile[cite: 1]
Local Setup & InstallationClone the repository:Bashgit clone [https://github.com/midhuneshbraj123/Jarvis.git](https://github.com/midhuneshbraj123/Jarvis.git)
cd Jarvis/my-slack-bot
Install dependencies:Bashnpm install
Configure environment variables:
Create a .env file inside the my-slack-bot directory and add your Slack API tokens[cite: 1]:Code snippetSLACK_BOT_TOKEN=xoxb-your-bot-token
SLACK_APP_TOKEN=xapp-your-app-token
Run the bot locally:Bashnode index.js
When running successfully, the console will log: ⚡ Bot is running!   24/7 Deployment on NestTo keep Jarvis online continuously using PM2:Bashpm2 start index.js --name "jarvis-slack-bot"
pm2 save
LicenseBuilt for the Hack Club Stardance Challenge.


