# Edpuzzle Answers Script
<img src="https://raw.githubusercontent.com/ading2210/edpuzzle-answers/main/static/images/screenshot4.png" alt="A screenshot of the generated webpage" width="500"/>

This bookmarklet can fetch the answers for the multiple choice questions on any Edpuzzle assignment. It can also skip the entire video, as well as automatically answer the questions and change the video speed.

Discord server: [edpuzzle.hs.vc/discord.html](https://edpuzzle.hs.vc/discord.html)

## Contents:
  - [Demo](#demo)
  - [Features](#features)
  - [Limitations](#limitations)
  - [Copyright Notice](#copyright-notice)
  - [Creating the bookmarklet](#creating-the-bookmarklet)
  - [Using the bookmarklet](#using-the-bookmarklet)
  - [Credits](#credits)

## Demo: 
https://user-images.githubusercontent.com/71154407/199671842-c3016f8c-8c7f-4526-b274-5bdd48f3a131.mp4

Note: This video was recorded with an older version of the script, so the GUI shown is missing some features.

## Features:
 - Can fetch and display the multiple-choice answers for any Edpuzzle assignment
 - Can automatically answer all the multiple-choice questions in an assignment
 - Includes a video skipper which allows for arbitrary navigation within an assignment
 - Has a tool to change the video speed
 - Has an option to prevent auto-pausing the video when the tab is hidden
 - Shows various stats about the assignment
 - Has a decent looking GUI
 - No login or extension required
 - Uses about:blank so it doesn't go into your browser history
 - Works on private Edpuzzle videos
 - Supports Edpuzzles embedded in Canvas and Schoology
 - Licensed under the GNU GPL v3 license

Available now from our [Discord server](https://edpuzzle.hs.vc/discord.html): *An open beta of a completely overhauled GUI, with proper mobile support, ChatGPT integration for open-ended questions, and more.*

## Limitations:
 - This isn't able to answer open-ended questions or audio responses. Though in the future, I might use something like ChatGPT to complete those automatically. 
 - This doesn't currently work for most Edpuzzles that are embedded in a third party site. However, the script does work for Edpuzzles embeded in Canvas and Schoology.

## Copyright Notice:
This project is licenced under the [GNU GPL v3](https://github.com/ading2210/edpuzzle-answers/blob/main/LICENSE). Thus, you are not allowed to:
 - Reupload any part of the source code without crediting this repository.
 - Fork this repository, then change or remove the license.
 - Fork this project without linking to your modified source code. 

Forking or redistributing code from this repository is fine, as long as you abide by the terms of the GPL. However, if you don't, then I have every right to submit a DMCA takedown. Also, please don't try to take credit for work that is not yours by changing or removing the credits. Editing a couple of lines to remove my name and reuploading it doesn't make you look cool.

## Creating the bookmarklet:
A video tutorial can be found [here](https://www.youtube.com/watch?v=zxZzB2KXCkw).

### Method 1:
 1. Navigate to [https://edpuzzle.hs.vc](https://edpuzzle.hs.vc).
 2. If you're on any Chromium-based browser, drag the button at the bottom of the page into your bookmarks bar.
 3. If you're on Firefox, right click on the button and then click "bookmark link."

### Method 2:
 1. Copy the following code into your clipboard:
 ```js
javascript: fetch("https://cdn.jsdelivr.net/gh/ading2210/edpuzzle-answers@latest/script.js").then(r => r.text()).then(r => eval(r))
 ```
 2. Right click on your bookmarks bar and click "add page."
 3. Set the name of the bookmark to whatever you want.
 4. Paste in the code into the box for the url and save the bookmark.

## Using the Bookmarklet: 
### On Regular Edpuzzles:
 1. Navigate to any Edpuzzle assignment.
 2. Make sure the url follows this format: `https://edpuzzle.com/assignments/{id}/watch`
 3. Click on the bookmarklet to run the script.
 4. If it doesn't work, make sure you allow popups from edpuzzle.com, then try again.

### Usage on Canvas:
 1. Navigate to the assignment on Canvas. The link should look similar to this: ```https://k12.instructure.com/courses/{id}/assignments/{id}```
 2. Click on the bookmarklet. The script should open the Edpuzzle assignment in a new tab.
 3. Re-run the bookmarklet to launch the full script.
 4. If this doesn't work, make sure you allow popups on both Edpuzzle and Canvas.

## Credits:
The code for the video skipper is based off of [this](https://github.com/ASmallYawn/EdpuzzleSkipper), with permission from the original author and some major refactoring.

All other code has been written solely by me, [ading2210](https://github.com/ading2210).

This code has been modified for faster use and bypass blocking systems.

This project is licensed under the GNU General Public License v3.0.
