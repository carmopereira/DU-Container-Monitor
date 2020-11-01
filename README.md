# DU-Container-Monitor

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen.jpg" />

<b>OVERVIEW</b><br>
This code is destined to Dual Universe game.<br>
This is a Container monitor for pure and ore materials. It can be used to monitor container percentages and it readouts. It was design to have a Container Hub element side each item.<br>
<br>
This HUD was designed for a Large Transparent Screen(or two). Each screen can gather 20 materials. It uses a Zone detector to turn up every board for optimal CPU usage.<br>
<br>
<b>HOW TO SETUP HUD:</b>

1. Place Main board
2. Place a Transparent Screen L or similar
3. Place a Relay
4. Deploy a Zone Detector and connect it to the Relay

-----------------------------

<b>MAIN BOARD:</b><br>
Slot1: CORE<br>
Slot2: SCREEN_A<br>
Slot3: SCREEN_B (optional)<br>
Slot4: DOOR1 (optional)<br>
Slot5: DOOR2 (optional)<br>
<br>
<b>INSTRUCTIONS:</b>
1. Link CORE (no need to rename slot to CORE because it will autodetect)
2. Link SCREEN_A and SCREEN_B if needed (2nd screen is optional)
3. Copy minified code from Main Board file, and past it under advanced options on board options.
NOTE: when you copy paste the code, it will rename slot1 to CORE and slot2 to SCREEN_A
4. Link Relay to board and detector zone or manual button for example (optional) (you can always turn the board manually)
5. Edit board parameters (setup refresh rate in seconds, containers default space, percentage min and max for red and green incicators)
6. For every ContainerHub you will need to rename it to: CH_1L_ACANTHITE
<br>
<b>Label:</b><br>
CH stands for ContainerHub<br>
1 for quantity of containers<br>
L for size of the container<br>
ACANTHITE for material type<br>
<br>
Change everything accordingly except CH.<br>Ex.: CH_3S_CARBON (you have 3 small containers with carbon), CH_6L_IRON (you have 6 large containers with iron)<br>
<br>
Material name always in CAPS. List: HEMATITE, IRON, BAUXITE, ALUMINIUM, COAL ,CARBON ,QUARTZ ,SILICON ,LIMESTONE ,CALCIUM ,ACANTHITE ,SILVER ,MALACHITE ,COPPER ,NATRON, SODIUM, PYRITE, SULFUR, PETALITE, LITHIUM, CHROMITE, CHROMIUM, GARNIERITE, NICKEL, GOLDNUGGETS, GOLD, RHODONITE, MANGANESE, CRYOLITE, FLUORINE, COBALTITE, COBALT, KOLBECKITE, SCANDIUM, COLUMBITE, NIOBIUM, VANADINITE, VANADIUM, ILMENITE, TITANIUM, OXYGEN, HYDROGEN, WARPCELL<br>
<br>

-----------------------------

<b>CUSTOM ORDER ON SCREEN:</b><br>

At system start() you will find two variables. <br>
local SCREENA = {m1,m2,m3,m4,m5,m6,m7,m8,m9,m10,m13,m14,m15,m16,m21,m22,m11,m12,m17,m18}<br>
local SCREENB = {m19,m20,m23,m24,m25,m26,m29,m30,m31,m32,m33,m34,m27,m28,m35,m36,m37,m38,m39,m40}<br>
<br>
This will define the order that materials are placed on screen. If you need an empty space use m0. You can also use m41 for oxygen, m42 for hydrogen and m43 for warpcells<br>
Please use it wisely.<br>
<br>
<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/material_list.jpg" />

-----------------------------
<b>EXTRA:</b><br>

If you want you could format first screen with 4 columns. You could use this setting if you are not planning to use any container hub over the screen. Just uncheck "UseContainerHub" at parameters, and reload board.

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen_nohubs.jpg" />

-----------------------------

<h1>Bonus Screen</h1>

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/bonus_screen.png" />

This is a HTML only board. Feel free to change the names to your liking.


-----------------------------

Credits
carmopereira

NOTE: Any issue, please contact carmo#1590 at Discord
