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
