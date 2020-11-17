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
5. Add a Databank and connect it to the board. (Databank is used to save User Config to ease upgrades)

-----------------------------

<b>MAIN BOARD:</b><br>
Slot1: CORE<br>
Slot2: SCREEN_A<br>
Slot3-6: SCREEN_B (optional) / DOOR1 (optional) / DOOR2 (optional) / Databank (optional - no need to rename it)
<br>
<b>INSTRUCTIONS:</b>
1. Link CORE (no need to rename slot to CORE because it will autodetect)
2. Link SCREEN_A and SCREEN_B if needed (2nd screen is optional)
3. Copy minified code from Main Board file, and paste it under advanced options on board options.
NOTE: when you copy paste the code, it will rename slot1 to CORE and slot2 to SCREEN_A (if you are using a second screen, just neeed to rename the slot to SCREEN_B)
4. Link Relay to board and detector zone or manual button for example (optional) (you can always turn the board manually)
5. Edit board parameters (setup refresh rate in seconds, containers default space, percentage min and max for red and green incicators)
6. For every ContainerHub you will need to rename it to: CH_1L_ACANTHITE
7. Link Databank (no need to rename slot to DB because it will autodetect)
<br>
<b>Label:</b><br>
CH stands for ContainerHub<br>
C stands for Container<br>
1 for quantity of containers<br>
L for size of the container<br>
ACANTHITE for material type<br>
<br>
Change everything accordingly except CH or C.<br>Ex.: CH_3S_CARBON (you have 3 small containers with carbon), CH_6L_IRON (you have 6 large containers with iron), C_1M_IRON (you have 1 M containers with IRON (the number one could be omitted, like C_M_IRON)<br>
<br>
Material name always in CAPS. List: HEMATITE, IRON, BAUXITE, ALUMINIUM, COAL ,CARBON ,QUARTZ ,SILICON ,LIMESTONE ,CALCIUM ,ACANTHITE ,SILVER ,MALACHITE ,COPPER ,NATRON, SODIUM, PYRITE, SULFUR, PETALITE, LITHIUM, CHROMITE, CHROMIUM, GARNIERITE, NICKEL, GOLDNUGGETS, GOLD, RHODONITE, MANGANESE, CRYOLITE, FLUORINE, COBALTITE, COBALT, KOLBECKITE, SCANDIUM, COLUMBITE, NIOBIUM, VANADINITE, VANADIUM, ILMENITE, TITANIUM, OXYGEN, HYDROGEN, WARPCELL<br>
<br>

-----------------------------

<b>CUSTOM ORDER ON SCREEN:</b><br>
<br>
At system start() you will find two variables (SCREENA and SCREENB). <br>
<br>
local SCREENA = {"HEMATITE","IRON","BAUXITE","ALUMINIUM","COAL","CARBON","QUARTZ","SILICON","LIMESTONE","CALCIUM",<br> "MALACHITE","COPPER","NATRON","SODIUM","CHROMITE","CHROMIUM","ACANTHITE","SILVER","PYRITE","SULFUR"}<br>
<br>
local SCREENB = {"PETALITE","LITHIUM","GARNIERITE","NICKEL","GOLDNUGGETS","GOLD","CRYOLITE","FLUORINE",<br> "COBALTITE","COBALT","KOLBECKITE","SCANDIUM","RHODONITE","MANGANESE","COLUMBITE","NIOBIUM","VANADINITE", "VANADIUM","ILMENITE","TITANIUM"}<br>
<br>
<br>
This will define the order that materials are placed on screen. If you need an empty space use m0. You can also use m41 for oxygen, m42 for hydrogen and m43 for warpcells<br>
Please use it wisely.<br>
<br>
-- LIST OF ORE/PURES: <br>
-- "HEMATITE","IRON","BAUXITE","ALUMINIUM","COAL","CARBON","QUARTZ","SILICON"<br>
-- "LIMESTONE","CALCIUM","MALACHITE","COPPER","NATRON","SODIUM","CHROMITE","CHROMIUM","ACANTHITE"<br>
-- "SILVER","PYRITE","SULFUR","PETALITE","LITHIUM","GARNIERITE","NICKEL","GOLDNUGGETS","GOLD"<br>
-- "CRYOLITE","FLUORINE","COBALTITE","COBALT","KOLBECKITE","SCANDIUM","RHODONITE","MANGANESE"<br>
-- "COLUMBITE","NIOBIUM","VANADINITE","VANADIUM","ILMENITE","TITANIUM"<br>
<br>
-- EXTRA MATERIALS TO USE: "OXYGEN", "HYDROGEN", "WARPCELL"<br>
<br>
-- On this next arrays you will place witch order you like<br>
-- Read always left to right, then next line.<br>
-- YOU CAN SET "EMPTY" if you need a blank space<br>
<br>
<br>
<br>

-----------------------------

<b>DOORS:</b><br>

If you are using doors, just need to link them to the board. Name the slots DOOR1 and DOOR2 (optional).<br>
Activate at parameters (UseDoors), and at the final function at System/start, edit the caracter names that will trigger the doors.<br>
<br>
-----------------------------
<b>EXTRA:</b><br>

If you want you could format first screen with 4 columns. You could use this setting if you are not planning to use any container hub over the screen. Just uncheck "UseContainerHub" at parameters, and reload board.

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen_nohubs.jpg" />

-----------------------------

<h1>Bonus Screen</h1>

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/bonus_screen.png" />

This is a HTML only board. Feel free to change the names to your liking.

-----------------------------

<b>CHANGE LOG</b><br>
v1.4 11 Nov 2020 - first time i remembered to create a log<br>
v1.7 17 Nov 2020<br>
    Major refactoring<br>
    Added DB for upgrade purposes (storing user configs)<br>
    Added (L / kL / kt) readout below progress bar<br>
    Added capability to read containers and container hubs ( C_1L_IRON or CH_1L_IRON)<br>
    Restored old terminology to setup screen variables. Ore/Pure names instead m1,m2,m3,etc...<br>
    Info readouts when screen is setup and no container/hub found<br>
    Correct order for T1,T2,T3,T4 when using 2 full screens/1 without "hubsonscreen"<br>
    Added showHudWidget variable. Please turn it to true for DEBUG purposes.<br>
    Added capability to have 10 containers in the name. (Ex.: CH_10L_HEMATITE)<br>
<br>
    Thanks to: Jericho,Archaegeo,Kumare,Tricky Trixy,-CML- Schoff for all input.<br>
v1.8 17 Nov 2020<br>
	Container "C_" now working as intended. You can use either C_L_IRON or C_1L_IRON (no meaning to say that the "one" container is 1.)
	If you name 2 containers with the same ore/pure it will sum values of the two (or more)
<br>
<br>
-----------------------------

Credits
carmopereira

A big thanks to Jericho :) Your help is gold

NOTE: Any issue, please contact carmo#1590 at Discord or at DU_CONTAINER_HUD channel on DU Open Source Initiative Discord Server https://discord.gg/tBteJZSQxe
