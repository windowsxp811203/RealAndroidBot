# Changelog

### RAB 1.9.0
Note for Polygon# Enhancer users: Every enhancer feature can be now used with a free enhancer key with effect from Polygon# Version 0.8.4 

You can follow the paid instructions for Polygon# if you want backend data support.

- RAB now save a file that contain locations of device. This will help RAB to do debugging when necessary 
- Turtwig, Pidgey added to maintain throwing height list
- Minor text fix
- Location query for Google Pixel 4, android 11, fixed
- Fix `name 'lat' is not defined` error
- Will no longer check for encounter position for PGSharp Paid users
- RPC update: Fix polygon paid data issue
- Fix Mod/HAL shiny detection. RAB wrongly detect Shiny for Mod/HAL users
- Added Chase after Pokemon (Polygon Paid Only)
- Fix: Quit unknown battle
- Fix: Clear item on start when item_management is disabled
- Added Duskull detection
- Pumpkaboo and Gourgeist form and value fix

### RAB v1.7.3
- Gen 8 Fix: Gen 8 Pokemon's stats are not shown

### RAB v1.7.2
- Telegram Fix: Snipe: PVP 100 rating not registered
- If there are more to check after snipe, RAB will not resume route but continue to check for next Pokemon
- Gen 8 Update

### RAB 1.7.1

**BREAKING CHANGE**
From v1.7.1 onwards, PGSharp users using sniper or nearby feed, **Joystick MUST be removed** (from PGSharp option)

- PGSharp: Attempt to fix not able to input search string
- Attempt to fix not able to get Android version
- Ensure it’s at “Me” Profile page before getting Player Level
- RAB will not auto favourite newly caught Pokemon if Mass Transfer is not enabled 
- PGSharp Enhance Mode Changes: **Joystick MUST be removed** (from PGSharp option)
- Pokemon Names updated to Gen 8 (Stats are not included yet)
- Telegram Snipe: If Pokemon does not match, CD is 1 sec before restart route
- GUI Bugs: Navigation and Screenshot offset takes the vague from screen offset. This is fixed
- Attempt to fix not zooming out after restart app


### RAB 1.7.0
- PGSharp: RAB will now throw straight ball if name is not detected
- Polygon Paid: Added chase after Incensed Pokemon. Good for event where certain Pokemon only appear when using incense. Auto activated when incense is used
- Minor Text Change
- PGSharp Paid: Skip Encounter Intro is now enabled. Please enable this option if you enable Skip cutscene options in your PGSharp setting 
- Added `PGSharp Reposition` option. Disable it if you do not want RAB to move the elements of PGSharp
- Added player level detection 
- Fix: When spinning for poke stop after run out of ball, RAB will get stuck if users use instant spin

### RAB 1.5.0

Changes: Odd number release will be public version and even numbers will be development version.
Example: 
`1.3.x, 1.5.x, 1.7.x, 1.9.x` <-- These will be public release
`1.4.x, 1.6.x, 1.8.x, 1.10.x` <-- These will be development/beta release

- Fix: Search string changes is not being use by RAB when doing Mass transfer
- Improvement: Tepig detection improvement
- Fix: GL and UL ratings cannot be changed
- RAB’s PGSharp Enhance Mode: Improve name detection
- Attempt to disconnect GoPlus if teleporting to snipe (However, suggestion is to disable GoPlus if doing snipping as HAL now has auto reconnect which break this function)
- More options added for Telegram Snipe: 
New Type: `by_cp_less`, `by_cp_more` Options: `cp`
New Type: `by_ivs` Options: `atk`, `def` and `sta`, optional: `cp`
New option: `snipe_limit`, applicable to all type  
- Fix: RAB will get stuck during mass transfer when there’s event Pokemon in selection
- PGSharp Paid: Fix stuck at Team Rocket
- Fix: Crash as trying to read saved image (Some machines)
- Added PVP Feed for Donors
- Fix: Crash when trying to teleport back to starting location
- Fix: Stuck at weather warning screen
- Added: Pinap Exclusive option. Only use Pinap on selected Pokemon 
- Original Pinap entry removed from default config.example.yaml
- Reduce chances of hitting pokestop (non team rocket) if auto go plus is enabled
- RAB’s PGSharp Enhance Mode: Skip searching for Pokestop if auto go plus is enabled
- PGSharp: RAB will now attempt to determine if Pokemon have move to left, right or fly/attack
- Adjusted throwing height, solving the issue of miss hitting the Pokemon 
- Fix: Your device is not in our system (which cause donation feed not working)
- Fix: GPS Joystick fail to teleport for Android 7 and below

### RAB 1.3.1
- Fix: Connecting or disconnecting Go Plus loop
- Fix: Polygon Paid: If Pokemon Inventory is full, RAB will get stuck at Pokemon Encounter 
- Fix: Deleting of items by number not working on some devices
- Possible fix for some devices that perviously work on 1.2.3 but not working on 1.3.0

### RAB 1.3.0
- Faster response during catching of pokemon for 1. PGSharp Free/Paid, 2. HAL/Pokemod Espresso in quick catch Mode 3. MAD in Speed Up(Ball shake only one time, quick catch in RAB should be disabled for this mode)/Quick Catch mode
- Minor changes to Non advance berry selection mode
- Attempt to fix PGSharp get location error
- (PGSharp Enhance/PGSharp 100IV Shiny Hunt Mode) RAB will attempt to move the elements on screen after restart
- Added DPI setting for those who want to manually change their DPI
- 3 days trial PGSharp 100IV Shiny hunt feature
- (MAD Enhancer) Will skip appraisal during Pokemon management
- Fixed: Adjusting Min Atk in catch settings will also adjust Min Sta
- Fixed: Adjusting Check Item Interval will also adjust rest bagful interval
- Minior GUI Text Fix
- Attempt to address not incubating new eggs problem
- Corrected/Updated stats for Pumpkaboo, Gourgeist, Xerneas, Yveltal
- (Rooted Solutions) RAB will disconnect GoPlus if it’s activated before teleporting
- Added mass transfer option
- (Polygon#) Now support nameplate `{default} LVL{lvl} {ivs}` for Pokemon detail page, RAB will not do appraisal if this is set as nameplate
- (Non PGSharp) If run out of balls, RAB will attempt to spin 50 pokestops before resume normal operation
- Fix offset not found error (Telegram Snipe)
- Attempt to fix clicking onto AR quest when it’s not completed, and get stuck
- Fix: Attempt to improve Zero ball detection
- PGSharp Enhance mode will be available for all PGSharp users.
- Fix: Tapping on Scan Pokestop Quest which will cause RAB to get stuck
- PGSharp Enhance Mode: RAB will teleport back to starting location if it run out of ball. Please set your starting location to a place full of poke stop before starting RAB.
- Auto Teamrocket win for PGSharp Paid (From PGSharp v1.24.1 onwards)
- Pokemon Management: When transfering Pokemon, RAB will limit what can be transferred by using search string. Default: `age0-1` (new Pokemon within 48hrs)
- Pokemon Management: If Quick catch is also enabled, RAB will go back to Pokemon Inventory and favourite the last caught Pokemon if it's eligible for keeping. Please ensure Pokemon Inventory is set to recent list for this to work. 
- New Option: Search String (For Pokemon Management)
- Some devices are unable to use search string, RAB will fall back to mass delete by selecting 9 pokemons at a time and transfer up till the max number of pokemon assigned to check
- Checking if pgsharp menu is open, close it to prevent accidently clicking it
- Fix Teamrocket crash for non pgsharp users. (<D39)
- Attempt to detect home screen map better for some phones
- Restart wait time for MAD adjust to 90 secs as it always restart on it's own
- Item Management now accepts values. `0 = Do not delete, 1 = Delete all,  More than 1 = No. 0f Items to remind`

### RAB 1.2.3
- Pokemon Management: RAB will now scroll Pokemon inventory page
- PGSharp: Detect shiny from overlay
- Fixed: HAL has no PvP information
- PGSharp enhanced mode extended to Monday, 31 May 2021 23:59:59 GMT
- Fix: v1.2.0 to v1.2.2 auto close. **Please update to this version.**

### RAB 1.2.2
- Fix PvP catch setting. UL was max 1500. Fixed to 2500
- Fix Pokestop priority always enabled bug
- PGSharp Shuno Hunting: Speed up tapping
- Shiny Hunting: Fix stuck at weather warning
- Shiny Hunting: Fix stuck at travel too fast message
- Improvement: Encounter speed for HAL 
- Increased chance of detecting Marill 
- Fix: v1.2.0 and v1.2.1 auto close. **Please update to this version.**

### RAB 1.2.0
- Updated PGSharp enhance mode vaild date till 27 May 2021
- Level will not be considered (during transfer) if it's unkown when doing Pokemon Inventory management
- Level will not be considered for None (or GPS Joystick only) user
- Added Default Location for Telegram Sniping. This is to tell RAB where to teleport to after teleport to check for snipping. This value should be the first coordinate of your GPX Route.
- Fix stuck at Pokestop for non auto spinning users
- Added: Attempt to calcualte Pokemon Level if RAB failed to get from screenshot. (Accuracy +- 0.5)
- (NEW) Basic MAD support. Ensure IV toast is enabled
- Fix: When keep lucky pokemon is enabled, shiny check will always be enabled. This causes RAB not catching pokemon but leave the screen immediately.
- Fix: RAB mistake pokemon page as egg hatch and tries to do transfer instead of catching it.
- **IMPORTANT** The condition to keep pokemon has changed back to the orginal default: Atk AND Def AND Sta AND Min Level. There's now an option if you want to use Or condition for Min Level.
- Fix: Polygon# Paid cooldown issue. RAB now uses your phone system location rather than in game location data.
- Added Disable Auto Restart Module option
- (PGSharp) Added 100IV Shiny Hunt Module. Please use only sniper feed for this option.
- Attempt to improve CP detection during apprisal (This will slow down overall apprisal detection, will explore for other methods in future).
- Telegram module is now enabled for PGSharp users. PGSharp users who donated can now login in with telegram to get the additional benifits after the trial period is over.
- Attempt to detect PGSharp icon
- Options that are not supposed to be enabled, are now disabled
- Minor Bug Fix

### RAB 1.1.2
- (Polygon# Paid Fix) Fix INVENTORY\_FULL looping
- (Polygon# Paid Fix) Faster tapping
- RAB will now auto zoomout if you didn't
- RAB will attempt to restart if prolong period of no activity
- Auto close Detail Page after restart
- (Non HAL) RAB will now just click minus (-) sign to delete all items
- Added zoom out method option. (Select pinch in or punch out to zoom out)
- Added advance berry check option. Only use it when RAB is not able to detect berries
- Added Enchanced PGSharp Mode. 
- 1. Enable nearby radar and flash it all the way to exterme left. 
- 2. The PHSharp icon flash all the to the right
- If auto goplus is not availible in Enchanced PGSharp Mode, RAB will look for a pokestop to spin after encounter a pokemon.
- Attempt to fix Pokemon Magement (transfer) feature.
- Fix RAB not searching and spinning pokestop in PGSharp Enhanced Mode
- Fix RAB not transfering on some devices
- Hidden Option: hyper\_mode. maanually add 'hyper_mode': true under 'client' option to activate it. This is to help to speed up some process. **Work in process, Work for some people only.**
- 1. Hyper Mode: Speed up closing of pokemon caught summary page for those without quick catch option.
- Minor Bug Fix

### RAB 1.1.1

This is a bug fix update. You are encourage to update to this version if you have issue with the telegram features.

We have now included a patch file update for RAB v1.1.1. If you already have RAB v1.1.0 installed, you can simply download the patch file, unzip and overwrite the files in your v1.1.0 RAB Folder. This is so that you don't have to redownload the 100+mb file all over again.

- Faster Gym detection
- Fix Index Out of Range
- RAB will now pasue for any key to show summary before exiting
- RAB will now ask user to select from list if there are more than one device detected
- UI Update. CTRL+C reminder now in RED
- Attempt to fix Egg Hatch but did not incubate new egg
- Attempt to fix not identifying encounter while claiming rewards in quest
- (Team Rocket) Slot Pokemon if there are any empty slots. RAB will no longer swipe at Team Rocket Encounter screen.
- Fix Telegram features not working on Windows

### RAB 1.1.0
Note that for this version, manual installation will need to re-run `pip install -r requirement.txt`. If you have not update to RAB 1.0.9 previously, you'll nned to run `pip install sourcedefender -U` too.

Bot is now faster but some people might have issue. RAB might not catch any pokemon. When that happens, set `Delay Time` under Configuration tab to 2.5 secs (if still cannot, increase 0.5 and test try again)

We welcome new translations. If you have your own translation, free feel to message RAB Admin in discord. 

- Adjust the scrolling for quest for phones with offset (To solve issue of quest that are done, but didn’t get cleared)
- (Polygon Enhancer Paid) Check for gyms with slots and attempt to slot pokemon.
- Attempt to reconnect Go Plus (If user have one or using HAL/PGSharp Paid’s virtual Go Plus)
- Fix: Stuck at “Going too fast” 
- Added `notify_all_encountered` option
- Time adjustment done for `None` preset (GPS Joystick with route) `None` Preset should now be fixed and users can choose to use this without any 3rd party. 
- Added Keep Event Pokemon 
- Telegram tab updated (GUI)
- Donation feed is now live. You can now use our telegram feed to do Shiny Hunting. Or even SHundo hunting. Instructions on how to donate is at Telegram Tab.
- German Translation partially updated.
- Fix (None Profile): Not able to detect catch page when encounter Pokemon during at quest page
- 720x1280 (720p) support. RAB will automatically detect and change to either 1080p or 720p base on what your phone support.
- Notify all encountered (Good to inform you what Pokemon RAB has seen if you are just doing shiny Tap)
- Fine tuning to various page detection
- Lower Resolution Option
- Farmer Discord Notification. Please note that all catch will be send to your webhook in this version. More options for farmer will be availible in next version
- Only one screenshot will saved/overwrite for new users. Existing users you can turn screenshot off by manually all the screenshot options in config.yaml to false
- Restart Pokemon Go if map is blank during shiny feed check (Polygon#).
- Fix starting quest check, “RAB didn't manage to tap into quest page” error
- Fixed None Profile (GPS Joystick only users)
- Summary when RAB quits
- Add delay timing option (will add more controls in future) for users with slower PC/Phones

### RAB 1.0.9

Note that for this version, manual installation will need to re-run `pip install -r requirement.txt`. You will also need to update your Source Defender by running `pip install sourcedefender -U`. You are also advised to delete your exisiting config.yaml before running the bot.

This version has multi-language support (GUI Only). If anyone interested to translate the GUI to your onw language, a german language example has been included in lang.yaml and you can use notepad++ to copy and paste to the end and change it your language.

Don't forget to send me a copy so that I can include it in next version.

- Fixed: RAB will mistaken pokemon still in catch page as caught/flee for quick catch users
- Fixed: pytesseract not found message for exe version
- Fixed: When there's a quest pokemon caught being done, RAB will ALWAYS click on pokeball. This is fixed
- Fix: Polygon will not auto close pokestop if it's under cooldown
- Bug Fix: Much quicker response time after catching a pokemon in quick catch (instant transfer) mode
- Added Graphical User Interface
- Multi-language support (GUI Only), German example is in current version (translated with Google Translate)
- Attempt to fix not getting Level
- RAB is now able to determine if a Pokemon is caught in quick catch mode. PGSharp user please enable caught preview.
- Config.example is now in rab folder
- RAB will auto create config.yaml if not found
- Attempt to fix stuck at team rocket leader
- Added learning ability to aid in identifying Pokemon (slightly more accurate over time)
- Attempt to fix not identifying poke ball on Windows machine
- Added `notify_all_caught` option to Discord webhook
- Updated getting IV from Appraisal. Should have improved results than v1.08
- Minor refinement of clicking positions
- If `power_up_lvl` is 0, RAB will now delete power quest
- Added Pokemon tracking for PGSharp and Pure GPS Joystick users (Client = None). This might not work all the time especially when the Pokemon starts to move before RAB can located it’s location
- Shiny was previously not reported to web hook in v1.08, this is fixed.
- RAB will now detect 0 balls. Will quit catch screen
- Added detection for 12 km egg
- RAB will quit if Pokemon Go is no longer running on phone.
- Added `last_quest_quit_today` option. RAB will move on when it encounter this given text in Today’s quest page. You are strongly advise to set `last_quest_quit_today`, `last_quest_quit` and `last_item_quit` if RAB get suck in these screens.
- Console will now show caught information for Polygon # paid user (Exp, candies,XL and stardust earned)

### RAB 1.0.8 Beta

**Note** Polygon Network mode is back! Only for Polygon# paid user. Free Polygon users please use `Polygon` for the client option and Paid user please use `Polygon Paid` as the option for client.  

- Added 'Polygon Paid' as an option for client
- Added back all the feature of Polygon# for Polygon# paid users
- Added `auto_offset` to config. Defaulted to `true`. RAB will now attempt to auto test your screen to see if it's compatible with RAB. It will then suggest some values where you can add them to your config file. You can then set `auto_offset` to false if you are happy with what RAB suggested to you.
- Bug Fix (PGSharp): Waited very long to throw a second pokeball
- Bug Fix: Pokemon Management will be messed up if there's a lucky pokemon
- Bug Fix: RAB will powerup level 1 pokemon despite quest set to false. This is fixed.
- Bug Fix: RAB will be stuck at a lot of places using snipe and shiny check feature
- Bug Fix: Stuck at collect component screen

### RAB 1.0.7
**NOTE:** Due to the recent announcement by Polygon#, we will be removing Network mode of Polygon# from RAB. What does this mean? It mean Polygon# users will no longer be able to teleport to exactly where pokestops/pokemon are. No longer able to automatically capture shiny or 100 Polygon# found. All features of Polygon# will be removed.

Due to this sudden changes, we are unable to fully optimize support for Polygon# users and you might see your avatar stuck at different places frequently. As such I suggest you switch to Pokemod temporary.

- Added send enounter/caught information to Discord
- Changed default `spin_pokestop` from false to true
- Bug Fix: Team Rocket manage pokemon button not recognized 
- Bug Fix: Not feeding berries
- Auto scripts for Windows User to simplify installation process
- Remove network setting for Polygon#. Now Polygon# will work just like HAL. 
- Options orginally meant for Polygon# are removed
- Added only_shiny mode. Also known as shiny tap. It will only catch if poke is shiny, else flee.
- Added navigation_offset option. For phones with buttons and you can't disable/remove them, we now have an option for you to remove it. Set the height of your navigation bar here.

### RAB 1.0.6
- Added Pokemon Inventory Mangement. RAB will now auto keep or release pokemon in your bag when it is full
- New options for Pokemon Inventory Mangement are `enable_poke_management`, `manage_poke_on_start`, `inventory_iv` and `stop_check_at`. Please check config.example.yaml and update your exising config accordingly.
- `keep_strong_shadow` and `keep_legendary` options added under catch

### RAB 1.0.5
- PGSharp is now fully supported. Paid users try to shift your joystick to somewhere that wont be click on or block important text.
- Added `auto_route` option under `client`. PGSharp free users and Polygon# users please set this to false. PGSharp Paid users please set this to true if using auto walk or route.
- Added `screen_offset` option. Some phones, especially those with front camera build right atb the top middle of the screen, certain page in Pokemon Go will be shifted slightly downwards. To test if you need to add a number here, set clear_item_on_start to true, and see if the name of the items are correctly captured. If not, set a number here or seek help in discord. (try 80)

### RAB 1.0.4
- Added PGSharp (Free Version) Support. 

### RAB 1.0.3
- Added Polygon Support. (Please do `pip install -r requirements.txt` to get new requirements needed.
- Added client type option in config.
- Added network settings. (Polygon Only)
- Added `stop_at_ball` and `resume_at_ball` options (Polygon Only)
- added `catchpoke_every_x_spin` option. Catch a poke in between x pokestop spinning. (Polygon Only)
- Snipe support for Polygon#. Works differently from Pokemod/HAL. (Snipe is still not availibe for public, more information will be release in our Discord Channel)
- Auto catch shiny Pokemon detected by Polygon. (Polygon Only)
- Added `last_item_quit` to item_management option. Set something here for the bot to know when to quit item page. Example set to `Incense` and RAB will auto quit when it see Incense in item page
- Added `last_quest_quit` to quest option. RAB will auto quit when it sees the key word here. Example, if you set to `Mythical`, RAB will quit special research page when it sees the quest A Mythical Discovery.

### RAB 1.0.2r2
- Hot Fix: Auto Max (HAL Only)

### RAB 1.0.2r1
- Hot Fix: Stuck at berry selection page

### RAB 1.0.2
- If `manual_set_resolution` is set to true, exiting bot will no longer change screen resolution
- Added `power_up_lvl` to config. How many times do you want to powerup a level 1 pokemon.
- Added `select_ball` to config. Default auto select ball. Set to false to use default ball without selecting
- Speed up catching for users using `transfer_on_catch` options

### RAB 1.0.1
- Added `use_berry` option, defaulted to true
- Added `manual_set_resolution`, defaulted to false

### RAB 1.0
- First Commit