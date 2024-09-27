# Twitch Gif Bot Overlay

This will allow Twitch chat to use a custom command like: "!gif  https://tw-pics.4lima.de/peace_puzzle.gif". 
It will then display the image from the user. 

including 2 versions for use

- gif_overlay.html	-> shows the images in fullscreen btw. how big you made the overlay in your OBS...
- gif-border-include_overlay.html	-> the name say´s all. there is a border included as base64image...

## Requirements and notes

This project can run locally and does not require a server. 

This requires a Twitch Account for use!

## Install and use

### 1.Simple way

Simply open the *.html in a web browser 
and add the following after the .html 
`?channel=YOURCHANNEL`.



### 2.Advanced way

- Open *.html in a text editor like notepad++
- Look for this section. 

```		// Configuration - Settings
		// if you have problems to add the channel in adressfield of OBS uncommand following line:
		//let twitchChannel = "YOURCHANNEL";
		let twitchChatCommand = "!gif";
		let defaultImage = "";
		let borderImage = "";
		let timeOut = 10;
```

- twitchChannel: Required. Your Twitch channel name.
- twitchChatCommand: Required. The Twitch chat command (!gif) is standard.
- defaultImage: Optional. This will set a background image. This could be an image that you want to display when no Gif images are being played.
- borderImage: Optional. This will set a personal border image. This shows an image in fullscreen that is used when Gif images are being played.
- timeOut: How long should the image stay on screen. Set this to 0 if you want to image to stay on screen until another image is played.

Once everything is configured and saved, you can now open *.html in your default web browser to test. 

Copy the URL from your browser to add it to OBS as a browser source... example: (file:///home/user/twitch_gif_overlay-bot/gif_overlay.html)