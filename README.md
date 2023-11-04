

### Cloudflare deploy
 * - Set [secret](https://developers.cloudflare.com/workers/configuration/secrets/) from Cloudflare dashobard
 * - Run `npm run deploy` to publish your worker
<!-- for logs -->
`wrangler tail`

###  Locally run
 * - Run `npm run dev` in your terminal to start a development server
 * - Open a browser tab at http://localhost:8787/ to see your worker in action
for running locally have `.dev.vars` file with 
# BOT_TOKEN='telegram bot token'
# CHAT_ID='your telegram chat id'


<!-- for creating app -->
npm create cloudflare@latest
