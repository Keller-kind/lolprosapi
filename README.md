# lolprosapi

lolprosapi is a simple api that shows your viewers which Pro Players are in your game and responds with a String in the format {name} ({champ}, {tag} {main_position}) | {name} ({champ}, {tag} {main_position}) | {name} ({champ}, {tag} {main_position}) etc. , hence it can be used to interact with chatbots like nightbot, moobot, fossabot etc.

## Usage

To use lolprosapi, simply add a command that only has a urlfetch to your chatbot.

### Nightbot
`!addcom !players $(urlfetch http://api.poldi.cloud/your_name)`

### Moobot
- If you know how to add commmands via text you know how to do a urlfetch
- If you don't, add a new Command via the website
- Choose Advanced Options
- Choose `URL fetch - Full (Plain) Response` as Response type
- add `http://api.poldi.cloud/your_name` as URL to fetch
- Request Method should be 'GET'
- URL Response Type should be 'Plain Text'
- Add Command

### Fossabot
idk, something with $(customapi)


## Disclaimers

**NOTE** that you should replace your_name with your name.

**NOTE** that this should be the name you're listed with on lolpros(**NOT YOUR LEAGUE ACCOUNT NAME**).

**NOTE** that this API only works if you are listed on lolpros yourself and the Account you're playing on is listed.
 
This only works if you are listed on lolpros as this API simply scrapes lolpros and formats a response.

Special Characters in your name are currently not supported.

If your Response is `Player not in Database`, check if your name corresponds with your name that your listed with on lolpros and doesn't have any special characters.
When you're sure you've done everything right, either wait a few days or weeks and retry, send me a message or open an issue in this repository.

This API might fail sometimes, as lolpros might be loading slow and most chatbots have a timeout of 10 Seconds. This might Result in your chatbot responding with an Error.
Just try again.



## Checklist
- You are listed on lolpros
- The Account you're playing on is listed on lolpros
- You added your Command with the correct name
- Your lolpros name doesnt have any special characters
- You have read the whole documentation
