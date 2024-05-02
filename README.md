 # Building Destroyer

This project develops a destructible building simulation for augmented reality (AR) environments on the Meta Quest 3 platform. It leverages hand tracking and physical effects that respond to hand movements for interactive building destruction.

Model: The building model is sourced from Unity assets available online. Upon launching the app, the model appears on the ground in front of the player. Players can then interact with the structure, initiating destruction by touching it with their hands.

Main Gaming Logic:(You can see code details in DestructableBuilding.cs) The building model is structured in two layers: a complete building overlay and underlying fragmented components. Initially, the complete building is visible. Upon detecting the first touch, the complete model is hidden, revealing the fragmented structure. This transition triggers a particle effect at the point of impact, applying a force that simulates destruction. The logic also applies to collisions with specific building components.

Installation Instructions:

1. Download the BuildingDestroy.apk file through this link: https://drive.google.com/file/d/1bDZGHzRQq1-ynZQdPFDuZC-zscj5sLqq/view?usp=drive_link .
2. Install the APK using SideQuest on a desktop.
3. Launch "My Project(1)" from the "Unknown Sources" section in the library on a Meta Quest 3 device synced with SideQuest.

(Note: This application has only been tested on Meta Quest 3; compatibility with other Android-based platforms is not guaranteed.)

Future Development Goals:

1. Expansion to City-Scale Destruction: The current work is only part of the initial plan. The original plan was to create a whole destructible city, but due to the high cost of building models and their fragmented versions, I ended up making only one building as a demonstration. If I copy the model multiple times and adjust the parameters, I can achieve the effect of a city, but it will still appear that all the buildings in the city are too similar. Therefore, my future goal is to create a realistic city (rather than a basic 3d building model) to destroy.
2. Enhanced Destruction Effects: Improve the realism of the destruction effects, specifically the explosion visuals, to provide a more immersive experience.
3. Gameplay Complexity: Introduce enemy interactions, such as shooting, requiring players to dodge attacks while engaging in destruction.
4. Room Scanning Integration: Although I implemented the scanning of rooms through meta quest3 in the previous milestone, I encountered difficulties when applying the scanned room model. In the future, I plan to solve this problem so that the simulated city can appear on designated furniture (such as sofas, tables), not just on the ground.


