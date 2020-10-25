# DU-Container-Monitor

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen.jpg" />

<b>OVERVIEW</b><br>
This code is destined to Dual Universe game.<br>
This is a Container monitor for pure and ore materials. It can be used to monitor container percentages and it readouts. It was design to have a Container Hub element side each item.<br>
<br>
This HUD was designed for a Large Transparent Screen(or two). Each screen can gather 20 materials. It uses a Zone detector to turn up every board for optimal CPU usage.<br>
<br>
<b>HOW TO SETUP HUD:</b>
1. Place a Relay
2. Place a Transparent Screen L or similar
3. Place Main board
4. Deploy a Zone Detector and connect it to the Relay

-----------------------------

<b>MAIN BOARD:</b><br>
Slot2: SCREEN
Slot3: DOOR1 (optional)
Slot4: DOOR2 (optional)

<b>INSTRUCTIONS:</b>
1. Connect CORE (no need to rename slot to CORE because it will autodetect)
1. Connect SCREEN_A and SCREEN_B if needed (you will need to rename the slots to SCREEN_A and SCREEN_B)
3. Connect Relay to board
4. Copy minified code from Main Board file, and past it under advanced options on board options
5. Edit board parameters (setup refresh rate in seconds, containers default space, percentage min and max for red and green incicators)
6. For every ContainerHub you will need to rename it to: CH_1L_ACANTHITE

Label:
CH stands for ContainerHub
1 for quantity of containers
L for size of the container
ACANTHITE for material type

Change everything accordingly except CH.

Material name always in CAPS. List: HEMATITE, IRON, BAUXITE, ALUMINIUM, COAL ,CARBON ,QUARTZ ,SILICON ,LIMESTONE ,CALCIUM ,ACANTHITE ,SILVER ,MALACHITE ,COPPER ,NATRON, SODIUM, PYRITE, SULFUR, PETALITE, LITHIUM, CHROMITE, CHROMIUM, GARNIERITE, NICKEL, GOLDNUGGETS, GOLD, RHODONITE, MANGANESE

-----------------------------

<h1>Bonus Screen</h1>

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/bonus_screen.png" />

This is a HTML only board. Feel free to change the names to your liking.


-----------------------------

Credits
carmopereira

NOTE: Any issue, please contact carmo#1590 at Discord
