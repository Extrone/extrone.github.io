---
title: "Editing Clocks"
summary: You can easily edit Timers and Stopwatches in the editor. Let's learn how.
url: "/plugins/editorclock/documentation/editingclocks"
weight: 150
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
Labels: [""]
Projects: ["Editor Clock"]
Engines: ["Unreal Engine"]
unrealengineversions: ["5.4", "5.5", "5.6"]
author: " "
cover:
    image: "EditorClockSave.png"
    alt: "Editor Clock Plugin Editing Clocks"
    relative: false
---

# Editor Clock Save
Clocks (Timers & Stopwatches) are saved in a Config file called `EditorClockSave.ini` in `[Plugins]/EditorClock/Config/` folder. <br>
It is also available through the Editor in `Editor Preferences -> Plugins -> Editor Clock Save`.

![Editor Clock Save](EditorClockSave.png)

## Editing a Timer
### In Engine
1. Open `Editor Preferences -> Plugins -> Editor Clock Save`
2. Find the Timer you want to edit in the `Timers` Array.
3. Through the Editor you can edit the `Name`, `Initial Time` and the `Current Time` of the Timer.
4. Editing the `Name` will only be applied after restarting the Editor.
### Outside Engine
1. Open `EditorClockSave.ini` file `[Plugins]/EditorClock/Config/` folder