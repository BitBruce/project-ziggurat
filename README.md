# About
I made a Discord chatbot for my friends one weekend and decided to strip all personal functions to create this skeleton-of-a-Discord-bot project. Feel free to contact me (or open an issue or pull request) if you have any questions or suggestions.

# Installation

1. `npm install`
1. Create a Discord bot on [Discord's developer site](https://discordapp.com/developers/applications/me)
1. Add bot to your Discord server
1. Supply API token in `.env` file (`DISCORD_TOKEN=your_api_token_here`)

# Run

- Supply discord api token in `.env` (Using `npm i dotenv`)
- `node z-bot.js`

# Development

[Discord.js documentation](https://discord.js.org/#/docs/main/stable/general/welcome)

## ToDo/Ideas

- Use MongoDB & Mongoose
- Dialogflow for ML chatbot

# Changelog
- v1.0 (04/23/18) - Release barebones app

---

### OAuth2 Example
*(Needed to set up Discord bot I think? Leftover from months ago)*

From https://github.com/discordapp/discord-oauth2-example

- Head over to [Discord's developer site](https://discordapp.com/developers/applications/me) to create an application, and then save the `client id` and `client secret` to use in OAuth2 libraries as `client_id` and `client_secret`.
- `cd /oauth`
- `pip install -r requirements.txt`
- `OAUTH2_CLIENT_ID=152638009253036032 OAUTH2_CLIENT_SECRET=p6KNMamrU5OVWtZiFe2kSkhx3Amxm0xB python app.py`
- `open http://localhost:5000`

#### Scopes

- **identify** allows `/users/@me` without `email`.
- **email** makes `/users/@me` return an `email`.
- **connections** allows `/users/@me/connections` to return linked Twitch and YouTube accounts.
- **guilds** allows `/users/@me/guilds` to return basic information about all of a user's guilds (servers).
- **guilds.join** allows `/invites/<code>` to be used to join a guild (server) with an instant invite.
