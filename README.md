# express-discord-oauth2
An example how to use discord's OAuth2 in express (node.js)

## Instalation
1. Install Node.JS [here](https://nodejs.org/)
2. To install the dependencies, run `npm install` (All dependencies are already listed in `package.json`)


## Configuration
* `port`: The port website will use
* `oauth2`:
  * `redirect_uri`: URI that you've been redirected after authorization in Discord
  * `client_id`: Your client's ID
  * `secret`: Your client's secret (**NOT TOKEN**)
  * `scopes`: Scopes that will be requested for user
  
  Discord's OAuth2 API docs: https://discord.com/developers/docs/topics/oauth2
* `session`:
  * `secret`: Secret code for `express-session`
  * `cookie`:
    * `maxAge`: Max age of cookies in milliseconds
  
  Other information about `session` config can be found [here](https://www.npmjs.com/package/express-session)
  

## Running
Before running: Make sure that you have been changed port, session config and oauth2 data in `config.json`

----------------
[!] **Important!** If you don't know how to use Discord's OAuth2 API read more about it here: https://discord.com/developers/docs/topics/oauth2
