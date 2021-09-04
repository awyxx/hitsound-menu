# Hitsound menu for Sourcemod

Forum link: https://forums.alliedmods.net/showthread.php?p=2756948#post2756948 <br>

How it works: https://www.youtube.com/watch?v=zVL-AnkvyMo&feature=emb_title <br>

### Stuff:
* .sp - Source code <br>
* .smx - Compiled plugin<br>
* sound/erasounds/ - Default hitsounds <br>

### Installation:
Put the .smx file into your plugins/ folder (in your server files)
I've also included some hitsounds by default, you have to move erasounds/ to your sound/ server folder.
*(Make sure your server's fastdl is working)* <br>

### Adding more hitsounds:
If you install this plugin correctly, it should have 12 hitsounds by default, if you want to add new hitsounds, you will have to edit and recompile the plugin.
But its pretty simple, follow the example below:
Lets say you want to add a new sound, which has this path: /myfolder/mysound.wav
You just need to add 2 lines!
```
char g_sounds[][] = {
	"",
	"play */erasounds/fdp_era.wav",
  "play */erasounds/cod_era.mp3",
  "play */erasounds/nojohit_era.wav",
  "play */erasounds/nojohittwo_era.wav",
	"play */erasounds/bubble_era.wav",
	"play */erasounds/bounce_era.wav",
	"play */erasounds/catgun_fire01_era.wav",
	"play */erasounds/firework_1_era.mp3",
	"play */erasounds/punch_era.mp3",
	"play */erasounds/laser_era.mp3",
	"play */erasounds/bonk.wav",
	"play */erasounds/bameware_era.wav",
	"play */myfolder/mysound.wav" // you just need to add this
};
char g_sounds_name[][] = {
	"None",
  "Skeet",
	"Cod",
	"Nojo1",
	"Nojo2",
	"Bubble",
	"Bounce",
	"Catgun",
	"Firework",
	"Punch",
	"Laser",
	"Bonk",
	"Bameware",
	"MySound" // and this
};
```

### TODO:
* Add hitsounds via config file
