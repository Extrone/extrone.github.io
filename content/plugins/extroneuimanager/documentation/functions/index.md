---
title: "Function Reference"
summary: Information on what every function in this plugin does.
url: "/plugins/extroneuimanager/documentation/functions"
weight: 2
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
Tags: ["Blueprint"]
Categories: ["Documentation"]
Projects: ["Extrone UI Manager"]
Engines: ["Unreal Engine"]
unrealengineversions: ["5.4"]
author: " "
cover:
    image: "Extrone_UI_Manager_Functions_Thumbnail.png"
    alt: "Extrone UI Manager Plugin Getting Started"
    relative: false
---

## Initialize Extrone UI Manager
Initialize ExtroneUIManager Subsystem

![*Screenshot of Initialize Extrone UI Manager Blueprint Node*](nodes/InitializeExtroneUIManagerBFL.png)

|In|Description|
|--|-----------|
|PlayerController|Player Controller that should own all the <br> Layers and Screens Created by Extrone UI Manager|

## Push Screen To Layer
Creates and pushes provided screen class to selected Layer

![*Screenshot of Push Screen To Layer Blueprint Node*](nodes/PushScreenToLayerBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer to which the Screen should be pushed to|
|ScreenClass|Widget Class that should be created and pushed to Layer|

|Out|Description|
|---|-----------|
|ScreenWidget|Widget that was created and pushed to the Layer|
|bSuccess|True if ScreenWidget was successfully pushed to Layer|

## Push Screen Widget To Layer
Pushes provided Screen to selected Layer

![*Screenshot of Push Screen Widget To Layer Blueprint Node*](nodes/PushScreenWidgetToLayerBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer to which the Screen should be pushed to|
|ScreenWidget|Widget that should be pushed to Layer|

|Out|Description|
|---|-----------|
|bSuccess|True if ScreenWidget was successfully pushed to Layer|

## Pop Screen
Pops the provided Screen from its layer if it's the Top Screen on that Layer

![*Screenshot of Pop Screen Blueprint Node*](nodes/PopScreenBFL.png)

|In|Description|
|--|-----------|
|ScreenWidget|Widget that should be popped from its Layer <br> (Automatically set to Self if parent class is UExtroneScreenBase)|

|Out|Description|
|---|-----------|
|bSuccess|True if the Screen was popped successfully|

## Pop Top Screen From Layer
Pop the Top Screen from provided Layer 

![*Screenshot of Pop Top Screen From Layer Blueprint Node*](nodes/PopTopScreenFromLayerBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer from which it's top Screen should be popped|

|Out|Description|
|---|-----------|
|ScreenWidget|Widget that should be popped, if it's the Top Screen of the Layer|
|bSuccess|True if the Top Layer was popped successfully|

## Clear UI Layer
Remove all Screens from provided Layer

![*Screenshot of Clear UI Layer Blueprint Node*](nodes/ClearUILayerBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer that should be cleared|

|Out|Description|
|---|-----------|
|bSuccess|True if the Layer was cleared successfully|

## Get Top Screen On Layer
Get the Top Screen from selected Layer if it has any Screens

![*Screenshot of Get Top Screen On Layer Blueprint Node*](nodes/GetTopScreenOnLayerBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer from which to get the Top Screen from|

|Out|Description|
|---|-----------|
|ScreenWidget|Top Screen Widget of Layer if it had any screens|
|bIsValid|True if ScreenWidget is valid|

## Register UI Layer
Create and Register new Layer with provided Widget Class

![*Screenshot of Register UI Layer Blueprint Node*](nodes/RegisterUILayerBFL.png)

|In|Description|
|--|-----------|
|Layer|GameplayTag that should be used to Identify this Layer|
|LayerWidgetClass|Base Widget that the screens will be pushed to|
|ZOrder|ZOrder of the Layer|

|Out|Description|
|---|-----------|
|bSuccess|True if new Layer was registered successfully|

## Register UI Layer Widget
Register new Layer with provided Widget

![*Screenshot of Register UI Layer Widget Blueprint Node*](nodes/RegisterUILayerWidgetBFL.png)

|In|Description|
|--|-----------|
|Layer|GameplayTag that should be used to Identify this Layer|
|LayerWidget|Base Widget that the screens will be pushed to|
|ZOrder|ZOrder of the Layer|

|Out|Description|
|---|-----------|
|bSuccess|True if new Layer was registered successfully|

## UnRegister UI Layer
Unregister provided Layer

![*Screenshot of UnRegister UI Layer Blueprint Node*](nodes/UnRegisterUILayerBFL.png)

|In|Description|
|--|-----------|
|Layer|that should be Unregistered|

|Out|Description|
|---|-----------|
|bSuccess|True if the Layer was Unregistered successfully|

## Set UI Layer Visibility
Set Visibility of provided Layer

![*Screenshot of Set UI Layer Visibility Blueprint Node*](nodes/SetUILayerVisibilityBFL.png)

|In|Description|
|--|-----------|
|Layer|Layer that's visibility that should be set|
|bVisible|Shows the widget if true otherwise hides it|

## Hide All UI Layers
Hides all UI Layers

![*Screenshot of Hide All UI Layers Blueprint Node*](nodes/HideAllUILayersBFL.png)


## Show All UI Layers
Shows all UI Layers

![*Screenshot of Show All UI Layers Blueprint Node*](nodes/ShowAllUILayersBFL.png)

## Is UI Layer Empty
Returns true if the selected Layer doesn't have any Screens

![*Screenshot of Is UI Layer Empty Blueprint Node*](nodes/IsUILayerEmptyBFL.png)

|In|Description|
|--|-----------|
|LayerTag|Layer that should be checked|

|Out|Description|
|---|-----------|
|bIsEmpty|True if the selected Layer doesn't have any Screens|

## Is Valid UI Layer
Returns true if selected Layer is registered

![*Screenshot of Is Valid UI Layer Blueprint Node*](nodes/IsValidUILayerBFL.png)

|In|Description|
|--|-----------|
|LayerTag|Layer that should be checked|

|Out|Description|
|---|-----------|
|bIsValid|True if selected Layer is registered|

## Get UI Layer Widget
Get the Widget that was registered to this Layer

![*Screenshot of Get UI Layer Widget Blueprint Node*](nodes/GetUILayerWidgetBFL.png)

|In|Description|
|--|-----------|
|LayerTag|Layer from which to get its widget|

|Out|Description|
|---|-----------|
|LayerWidget|LayerWidget that was registered to Layer|