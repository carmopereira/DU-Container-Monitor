# DU-Container-Monitor

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen.jpg" />

<b>OVERVIEW</b><br>
<br>
Container board v1.1 __ 14/10/2020<br>
Main board v1.0 __ 14/10/2020<br>
<br>
This code is destined to Dual Universe game.<br>
This is a Container monitor for pure and ore materials. It can be used to monitor container percentages and it readouts. It was design to have a Container Hub element side each item.<br>
<br>
This HUD was designed for a Large Transparent Screen. Each screen can gather 20 materials. It uses a Zone detector to turn up every board for optimal CPU usage.<br>
It has definition for current ore/pure types: Bauxite/Aluminium, Hematite/Iron, Quartz/Silicon, Coal/Carbon, Pyrite/Sulfur, Petalite/Lithium, Acanthite/Silver, Malachite/Copper, Limestone/Calcium and Natron/Sodium  [More to come in a few days]
<br>
<b>HOW TO SETUP HUD:</b>
1. Place a Databank
2. Place a Relay
3. Place a Transparent Screen L or similar
4. Place at least 1 board for containers and connect it to the Relay (blue link)
5. Place Main board and connect it to the Relay (blue link)
7. Deploy a Zone Detector and connect it to the Relay (blue link)
6. Deploy Doors (optional)(and connect them to the main board)

-----------------------------

<b>CONTAINER BOARD:</b><br>
Slot1: DB (databank)
Slot2: Material name in caps or SCREEN (optional)
Slot2 - slot10: Material name in caps

<b>INSTRUCTIONS:</b>
1. Connect DB
2. Connect Relay to board
3. Connect containers/Hub Containers to board (remember the order of the materials you connect)
4. Copy minified code from Container Board file, and past it under advanced options on board options
5. Edit board parameters (setup refresh rate in seconds, rename each slot to match ore/pure name you previously connected. Ex.: "HEMATITE", "BAUXITE", "IRON"

-----------------------------

<b>MAIN BOARD:</b><br>
Slot1: DB (databank)
Slot2: SCREEN (large transparent screen or similar)
Slot3: DOOR1 (optional)
Slot4: DOOR2 (optional)

<b>INSTRUCTIONS:</b>
1. Connect DB
2. Connect SCREEN_A
3. Connect Relay to board
4. Copy minified code from Main Board file, and past it under advanced options on board options
5. Edit board parameters (setup refresh rate in seconds and container default space)


-----------------------------

Credits
carmopereira

NOTE: Any issue, please contact carmo#1590 at Discord
