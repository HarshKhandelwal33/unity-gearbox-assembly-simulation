# Unity Gearbox Assembly Simulation

Unity simulation of a robot and worker assembling a planetary gearbox, controlled by a behaviour tree.

## Run

1. Clone this repository or download and extract it.
2. In Unity Hub, choose Add project from disk and select this repository folder (the folder containing Assets, Packages, and ProjectSettings).
3. Open with Unity **6000.6.0f1** and wait for asset import and script compilation.
4. Open **Assets/Scenes/GearboxAssembly.unity**.
5. Press the Unity **Play** button. The twelve loose components start on the rack and the assembly sequence runs automatically.

Double-click the Game tab to enlarge the preview. Move the Game view Scale slider left if the frame is cropped.

Controls: **Space** pauses/resumes, **R** resets, and **C** cycles cameras. The on-screen buttons provide Play/Resume, Pause, Step, Reset, Camera, and playback speed. After Reset, press Play/Resume to restart.

## Contents

This repository contains the prepared scene used for the running preview, including its models, materials, scripts, package manifest, and Unity settings. Generated caches are excluded and Unity recreates them on first open.

See GAME_SIMULATION.md for the behaviour tree, motion implementation, and limitations. game-simulation-report.txt records the existing automated checks for all 13 operations, ten handovers, all twelve installed parts, pause, reset, replay, and single-step. These checks were run against the source preview project before packaging.

The simulation uses kinematic animation and inverse kinematics; it is not a force/torque or collision-planning validation.
