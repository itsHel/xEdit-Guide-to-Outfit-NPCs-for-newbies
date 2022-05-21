# xEdit Guide to Outfit NPCs for newbies
Only prerequisite is to have installed _xEdit_
As example I will use [Sybille Stentor](https://en.uesp.net/wiki/Skyrim:Sybille_Stentor) and dress her in [Raven Witch Armor](https://www.nexusmods.com/skyrimspecialedition/mods/37878) using SSEEdit

## 1. Get NPC
The easiest way is to find your NPC on [uesp.net](https://en.uesp.net/wiki/Main_Page) and get it's __BaseID__ aka __FormID__
![img](/images/1.png)

If your NPC is from another mod you have two options
 - click on it ingame with [More Informative Console](https://www.nexusmods.com/skyrimspecialedition/mods/19250)
 - open your mod in __xEdit__ and find NPC by name manually under __Non-Player Character (Actor)__

Search your __BaseID__ in __FormID__ input (top-left), now you rightclick top of last column and select `Copy as override into`
![img](/images/3.png)

Select <new file>.esp (if you are doing this again just select your patch) and pick name, I will name it __myPatch__
![img](/images/4.png)

## 2. Create outfit
Scroll down to __DOFT - Default outfit__ property, click on it, copy it by `Ctrl + C` and paste it into __FormID__ input but it copied whole string so you need to clear it to be left with only 8 digits
![img](/images/5.png)

Now you rightclick outfit and select `Copy as new record into` and select your new mod (you could copy any outfit, it doesn't matter), I will name it ravenOutfit
![img](/images/6.png)

Go to __Armor__ category of mod which contains your armor and save __FormID__'s of all armor pieces you want to equip (You can click on box and use `Ctrl + C`)
![img](/images/7.png)

Now rightclick your mod, select `Add masters` and select mod which contains your armor
![img](/images/8.png)
 
Now go to your outfit and replace current items in outfit with your saved __FormID__'s
![img](/images/9.png)

If you need to add more items than outfit already contains you have to add new
![img](/images/10.png)

## 3. Finalize
Copy __FormID__ of your outfit and use it to replace NPC's current outfit
![img](/images/11.png)

Now just `Ctrl + S` to save your mod, don't forget to activate it in your modlist

And here she is
![img](/images/12.jpg)
