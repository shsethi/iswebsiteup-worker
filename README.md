# iswebsiteup

```
 _                  _         _ _                   
(_)                | |       (_) |                  
 _ _____      _____| |__  ___ _| |_ ___ _   _ _ __  
| / __\ \ /\ / / _ \ '_ \/ __| | __/ _ \ | | | '_ \ 
| \__ \\ V  V /  __/ |_) \__ \ | ||  __/ |_| | |_) |
|_|___/ \_/\_/ \___|_.__/|___/_|\__\___|\__,_| .__/ 
                                             | |    
                                             |_|    

```

## Description

This project is a Cloudflare worker that runs on a cron schedule and then interacts with a Telegram bot to alert the user. It can be deployed directly from your local environment to Cloudflare.

## Prerequisites

- Node.js and npm installed on your local machine
- A Cloudflare account
- A Telegram bot token and chat ID


## Setup

- Clone the repository to your local machine.
- Navigate to the project directory.
- Run `npm install` to install the necessary dependencies.

### Deployment to Cloudflare

- Set up your Cloudflare [secret](https://developers.cloudflare.com/workers/configuration/secrets/) from the Cloudflare dashboard.
- Run `npm run deploy` to publish your worker to Cloudflare.
- To view the logs, run `wrangler tail.`

### Local Development
- Create a `.dev.vars` file in the root directory of the project with the following content:

```sh
BOT_TOKEN='telegram bot token'
CHAT_ID='your telegram chat id'

```

- Replace 'telegram bot token' and 'your telegram chat id' with your actual Telegram bot token and chat ID.


- Run `npm run dev` in your terminal to start a development server
- Open a browser tab at http://localhost:8787/ to see your worker in action


### Contributing
Contributions are welcome!

### License
This project is licensed under the terms of the MIT license.