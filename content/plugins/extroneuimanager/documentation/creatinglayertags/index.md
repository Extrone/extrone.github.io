---
title: "Creating Layer Gameplay Tags"
summary: Need to add more Layer Gameplay Tags? Here is how.
url: "/plugins/extroneuimanager/documentation/createlayergameplaytags"
weight: 300
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
Projects: ["Extrone UI Manager"]
Engines: ["Unreal Engine"]
unrealengineversions: ["5.4", "5.5"]
programminglanguages: ["C++", "Blueprint"]
author: " "
cover:
    image: "Extrone_UI_Manager_Thumbnail.png"
    alt: "Extrone UI Manager Plugin"
    relative: false
---
## UI Layer Gameplay Tags
In Extrone UI Manager, Gameplay Tags are used to keep track of Layers.

## Default Layer Tags
By default the following Layer Tags are available
- ```UI.Layer.Game.World```
- ```UI.Layer.Game.HUD```
- ```UI.Layer.Game.Menu```
- ```UI.Layer.MainMenu```
- ```UI.Layer.HUD```

## Creating New Layer Tags
You can create Gameplay Tags using any of the [multiple ways](https://dev.epicgames.com/documentation/en-us/unreal-engine/using-gameplay-tags-in-unreal-engine) the engine provides, ***but make sure the tags have the Parent Tag*** ```UI.Layer```. (For example refer to Default Layer Tags)  <br> <br>

All Gameplay Tag properties and function inputs in Extrone UI Manager uses ```meta=(Categories="UI.Layer")```. 
This meta specifier filters the Gameplay Tags selection to the child tags of ```UI.Layer```. 
This makes it easier to find UI Layer tags. But it also means that you can't just use any Gameplay Tag as a Layer Tag.