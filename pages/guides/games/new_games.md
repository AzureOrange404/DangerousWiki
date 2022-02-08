---
layout: games
title: How To Games
description: Adding new Games to ES
light_mode: false
---

# How to add new Games
_by @RickDangerous_

1. Download skraper from [here](https://skraper.net/).
2. I choose _I have an account_ on the first screen if you don't, then choose _I don't have an account and I want to regsiter_ and hit sign up.

## Configuaration Wizard for Skraper

1. Choose Recalbox ( not RetroPie )
2. Select where you have your games on the pc.  
I store mine in d:\retro\roms
3. you don't have to select anything else just click next.
4. Click next on the default media screen.

## Skraper Usage

Now you are in the skraper program we can set it up as shown below.

1. Tick the box _Move Articles at the end of names_  
Optionally tick _Keep undercorated filename_

<div style="text-align: center;">
  
  ![Skraper Setup](../../../../assets/guides/games/add_games_1.png "Skraper Setup")
</div>

2. Select the Media Type: right facing  
3. arrow to change the first  
4. internal mix to video  
5. change the path %ROMROOTFOLDER%\media\videos to %ROMROOTFOLDER%\snaps

<div style="text-align: center;">
  
  ![Select Media Type](../../../../assets/guides/games/add_games_2.png "Select Media Type")
</div>

6. Change the media type box 3D to box 2D  
change the path from %ROMROOTFOLDER%\media\images to %ROMROOTFOLDER%\boxart

<div style="text-align: center;">
  
  ![Change Media Type](../../../../assets/guides/games/add_games_3.png "Change Media Type")
</div>

I recommend scraping one system at a time.

7. First select the system you wish to scrape on the left side.
8. Then hit the run button which is at the bottom right as shown below.

<div style="text-align: center;">
  
  ![Run Button](../../../../assets/guides/games/add_games_4.png "Run Button")
</div>

## Editing the Gamelist

Now the games have hopefully scrapped we can open the gamelist.xml and ensure everything is good. 
1. Locate the gamelist.xml in the systems folder you scrapped on your computer
2. Choose your favourite text editor to open the .xml file with. I personally use notepad++

<div style="text-align: center;">
  
  ![Gamelist.xml](../../../../assets/guides/games/add_games_5.png "Gamelist.xml")
</div>

### Rules I like to follow

- Check the game name is correct and matching to box art.
- Check Desc Tag should not be to long otherwise it will auto scroll and look messy!
- Check it has both image and video included
- Check atleast publisher or developer is included
- Check genre tag and change if needed to match one of the collections I use on the build.
- Check players tag is included.

If any of the tags are missing then I create them and get the information from online.
If no image or video tag included and you need to get your own image or video snap be sure to name is exactly as the rom name.
