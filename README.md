# Discord Invite in JS, HTML and CSS
A very-close-to-native Discord Invite script for websites.

Example:  
![Example of Discord Invite](example.png?raw=true "Discord Invite Example: Aegis7 Gaming")

miniMode Example:  
![Example of Discord Invite in miniMode](example-mini.png?raw=true "Discord Invite Example: Aegis7 Gaming (miniMode)")


## Why
Discord has this very minimlistic and practical invite box that tells users how many members a Discord server has, as well as how many users are online while giving the ability for that user to click a simple 'Join' button to, well, join the server.

As a huge fan of minimalist design and a fan of the Invite box, I thought it would be a good idea to make it possible to embed this on websites instead of the widget provided by Discord or the other solutions in the wild.

## How to use
 1. Download the files. (discordInvite.js, discordInvite.css)
 1. Upload the files to your web server.
 1. You will need an Invite Code that never expires from Discord.
 1. Include the CSS file in the head of the page:
    ```html
    <head>
    ...
    <link rel="stylesheet" href="/path/to/discordInvite.css"/>
    </head>
    ```
 1. Include the JS file and initialise on the page:
    ```html
    <body>
    ...
    <script src="/path/to/discordInvite.js"></script>
    <script>
      discordInvite.init({
      inviteCode: 'DQtcGRy',
      title: 'Aegis7 Gaming',
    });
    discordInvite.render();
    </script>
    </body>
    ```
1. Place this specific `<div>` wherever you want your invite to appear:
    ```html
    <div id="discordInviteBox"></div>
    ```

### Optional Values, default values are in (brackets)
`title` ('String')  
You can provide a default server name. The name will be replaced by whatever the invite code returns but it is good to have something there until the data is returned from Discord. Setting it to your current server name is a good idea.

`miniMode` (false)  
A cut down version of the invite box.

`width` ('385px')  
You can specify width as either 'auto', % or number (px). Alternatively, it can accept any CSS value as a string such as 'inherit' or '100w'.

`joinText` ('Join') and `joinedText` ('Joined')  
You can change the button text of the Join action to something else, as well as when the person clicks it.

`introText` ('YOU\'VE BEEN INVITED TO A SERVER')  
You can change the introText to something else.

`hideIntro` (false)  
You can hide the intro text

## Aegis7 Gaming
<a href="https://aegis7.com"><img src="https://aegis7.com/ag7logo.png" width=200></a>  
A gaming community with thousands of Discord users from all across the globe.  
[Join us on Discord: https://ag7.gg]

## No Support, 'as is'.
Please do not contact us for any support. We will do our best to provide updates when necessary and willing to accept pull requests but you should not expect us to fix issues for you, walk you through how to deploy this or anything of that nature.

## Discord
We are not affiliated in any way with Discord. We're just really big fans and we enjoy the platform! If at any time Discord and/or their staff tell us this isn't OK, we will take the script down. We're querying Discord servers and they can very well put this behind an Authentication layer, if this happens or the data is hidden or changed, this script will stop working; Please keep this in mind.
