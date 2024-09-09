# docs

### Resources
- [International Country Codes](https://www.worlddata.info/countrycodes.php), all use ISO Alpha2

## Setup Telegram
### 1. Setup Telegram bot
- Create a Telegram bot by following this [guide](https://core.telegram.org/bots#how-do-i-create-a-bot)
- [Linking your domain to the bot](https://core.telegram.org/widgets/login#linking-your-domain-to-the-bot)
- Get the bot token which has the format like this `[BOT_ID]:[BOT_API_TOKEN]`

### 2. Deploy `quest.aigo.network`
- Add `TELEGRAM_BOT_ID=[BOT_ID]` to `.env.production` in `aigo` repo
- Redeploy the `quest.aigo.network`

### 3. Deploy API
- Add `TELEGRAM_BOT_TOKEN=[BOT_ID]:[BOT_API_TOKEN]` to `.env.production` in `rocket` repo
- Redeploy the api

### 4. Add bot link to channel post
- Follow this [youtube guide](https://www.youtube.com/watch?v=OuWiP7tjIi4&t=414s) to add your bot to the channel
- Create the post through the bot
- In middle of the creating post process, add `URL Buttons` using this link [https://quest.aigo.network/#telegram](https://quest.aigo.network/#telegram)