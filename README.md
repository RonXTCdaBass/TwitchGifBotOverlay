# Twitch Gif Overlay Bot
## (final version 2025 with queue)

This will allow Twitch chat to use a custom command like: "!gif  FullURL/peace_puzzle.gif". 
It will then display the image from the user. 

download including 2 versions for use

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

* [LIVE-DEMO](https://tw-pics.4lima.de/GifOverlayBot/gob-combi.html?channel=YOURCHANNEL)
combi version - for fullscreen usage - my border and dvd screensaver like effect - change YOURCHANNEL - in demo you can switch the background ;)

----------

### 2.Advanced way

- Open *.html in a text editor like notepad++
- Look for this section. 

```
<!--/////////////////////////////////////////////////////////////////	
<// Configuration - Settings -instructions
<//
<// If the file is only to be used locally in OBS for a single fixed channel, 
<// please comment out the following paragraph between <-start ... & end-> tag and 
<// simply swap the two lines beginning with "let twitchChannel = ..." and 
<// enter the twitch channel. 
<////////////////////////////////////////////////////////////////////-->
```

- twitchChannel: Required. Your Twitch channel name.
- twitchChatCommand: Required. The Twitch chat command (!gif) is standard.
- defaultImage: Optional. This will set a background image. This could be an image that you want to display when no Gif images are being played.
- borderImage: Optional. This will set a personal border image. This shows an image in fullscreen that is used when Gif images are being played.
- PAUSE_DURATION: How many seconds between the various gif's? (3 * 1000 milliseconds)
- DISPLAY_DURATION: How long should every image stay on screen? (12 * 1000 milliseconds)

Once everything is configured and saved, you can now open *.html in your default web browser to test. 

Copy the URL from your browser to add it to OBS as a browser source... example: (file:///home/user/twitch_gif_overlay-bot/gif_overlay.html)

## Screenshot

![border_screenshot](https://github.com/RonXTCdaBass/TwitchGifBotOverlay/blob/main/border_screenshot.jpg)


------


