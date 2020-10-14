# DU-Container-Monitor by carmo

<img src="https://github.com/carmopereira/DU-Container-Monitor/blob/main/main_screen.jpg" />

<h1>OVERVIEW</h1>
Container board v1.1 __ 14/10/2020<br>
Main board v1.0 __ 14/10/2020<br>
<br>
This code is destined to Dual Universe game.<br><br>
This is a Container monitor for pure and ore materials. It can be used to monitor container percentages and it readouts. It was design to have a Container Hub element side each item.<br>
<br><br>
This HUD was designed for a Large Transparent Screen. Each screen can gather 20 materials. It uses a Zone detector to turn up every board for optimal CPU usage.<br><br>
It has definition for current ore/pure types: Bauxite/Aluminium, Hematite/Iron, Quartz/Silicon, Coal/Carbon, Pyrite/Sulfur, Petalite/Lithium, Acanthite/Silver, Malachite/Copper, Limestone/Calcium and Natron/Sodium  [More to come in a few days]
<br>
<h3>HOW TO SETUP HUD:</h3>
1. Place a Databank<br>
2. Place a Relay<br>
3. Place a Transparent Screen L or similar<br>
4. Place at least 1 board for containers and connect it to the Relay (blue link)<br>
5. Place Main board and connect it to the Relay (blue link)<br>
7. Deploy a Zone Detector and connect it to the Relay (blue link)<br>
6. Deploy Doors (optional)(and connect them to the main board)<br>

-----------------------------

<h1>CONTAINER BOARD:</h1>
Slot1: DB (databank)<br>
Slot2: Material name in caps or SCREEN (optional)<br>
Slot2 - slot10: Material name in caps<br>

<h3>INSTRUCTIONS:</h3>
1. Connect DB<br>
2. Connect Relay to board<br>
3. Connect containers/Hub Containers to board (remember the order of the materials you connect)<br>
4. Copy minified code from Container Board file, and past it under advanced options on board options<br>
5. Edit board parameters (setup refresh rate in seconds, rename each slot to match ore/pure name you previously connected. Ex.: "HEMATITE", "BAUXITE", "IRON"<br>

-----------------------------

<h1>MAIN BOARD:</h1>
Slot1: DB (databank)<br>
Slot2: SCREEN (large transparent screen or similar)<br>
Slot3: DOOR1 (optional)<br>
Slot4: DOOR2 (optional)<br>

<h3>INSTRUCTIONS:</h3>
1. Connect DB<br>
2. Connect SCREEN_A<br>
3. Connect Relay to board<br>
4. Copy minified code from Main Board file, and past it under advanced options on board options<br>
5. Edit board parameters (setup refresh rate in seconds and container default space)<br>


-----------------------------

<h1>Credits</h1>
carmopereira

<b>NOTE:</b> Any issue, please contact carmo#1590 at Discord
