# discord-id
discord id lookup tool - server to get info about discord id's

# Functionality & Features


User Info:


_username,
discriminator,
is system?,
is bot?,
tag,
profile picture,
account creation date,
badges,
nitro subscription status,
banner color
and account age._


Guild Info:


_name, splash url, description, total members, online members, profile picture, server creation date, features, and server age._


Logs the ip addresses, id's and request times both to the console and a text file.


Works with cross origin requests.


Provides both website and JSON API functionality.


Works no matter if the user has got their new username or not(discord discriminator removal update)
# Endpoints


/api/your-discord-id => Gives the info as JSON


/ => Asks for a discord id.


/info/ => Gives the info inside the website


# Usage & Setup
Install required dependencies:


`npm i fs express discord.js@13 consoled.js@1.0.4 ejs cors`


Get a discord bot token, then create an environment variable:


*export TOKEN="your-discord-bot-token"* for linux / mac


*set TOKEN="your-discord-bot-token"* for windows cmd 


*$env:TOKEN="your-discord-bot-token"* for windows powershell


This will secure your token on platforms like replit or codesandbox.


`node .` to start the server.

# Testing 


You can test the api [here](https://discord-id.rednexie.repl.co/)


for example, the url `https://discord-id.rednexie.repl.co/api/866793047596728321`


returns the response like 
*{


  "status": "success",

  
  "data": {

  
    "timestamp": "2021-07-19T21:26:06.783Z",

    
    "id": "866793047596728321",

    
    "username": "rednexie",

    
    "discriminator": "0",

    
    "system": false,

    
    "bot": false,

    
    "tag": "rednexie",

    
    "pfp": "https://cdn.discordapp.com/avatars/866793047596728321/ac6db6c5197c6eb46617f244c1a34cf1.jpeg",

    
    "createdAt": "19.07.2021 21:26:06",

    
    "timezone": "UTC",

    
    "badges": [

    
      "HOUSE_BRILLIANCE"

      
    ],
    "nitro": false,

    
    "bannerColor": "#ff0000"

  },
  
  "code": 200

}*



# Project Screenshots: 

<h2>Website</h2>

[https://camo.githubusercontent.com/c8f71d47218ef6d16d624c712cf642fb86690a5eda59e2ef5a18354dc88055fd/68747470733a2f2f7265646e657869652e6769746875622e696f2f456b72616e25323067254333254236722543332542436e7425433325424373254333254243253230323032332d30392d30342532303136323735362e706e67](https://discord-id.rednexie.repl.co/)


[https://camo.githubusercontent.com/5719c89c9f1a599a915855647535d65b96abb579084e43d0f770b3b149ed6d51/68747470733a2f2f7265646e657869652e6769746875622e696f2f456b72616e25323067254333254236722543332542436e7425433325424373254333254243253230323032332d30392d30342532303136323931332e706e67](https://discord-id.rednexie.repl.co/info/866793047596728321)


<h2>API</h2>

[https://raw.githubusercontent.com/Rednexie/rednexie.github.io/main/Ekran%20g%C3%B6r%C3%BCnt%C3%BCs%C3%BC%202023-09-04%20164308.png](https://discord-id.rednexie.repl.co/api/866793047596728321)



# Possible Updates

More logging options(mysql, perma.db)


Data storing/caching
