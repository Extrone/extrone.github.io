---
title: "Getting Started"
summary: Everything you need to know to start using the plugin.
url: "/plugins/extroneuimanager/documentation/gettingstarted"
weight: 100
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
Tags: [""]
Projects: ["Extrone UI Manager"]
Engines: ["Unreal Engine"]
unrealengineversions: ["5.4", "5.5"]
author: " "
cover:
    image: "Extrone_UI_Manager_GettingStarted_Thumbnail.png"
    alt: "Extrone UI Manager Plugin Getting Started"
    relative: false
---

## Installing the Plugin

1. Open Epic Games Launcher and navigate to **Unreal Engine → Library → Vault**
2. Search for **Extrone UI Manager**
3. Click Install to Engine and select the engine version you want to install the plugin to
4. Wait for the plugin to be downloaded and installed
5. Open your project and navigate to **Edit → Plugins**
6. Search for Extrone UI Manager
7. Enable Extrone UI Manager and Restart the Editor

## Initializing UI Manager Subsystem

Initialize Extrone UI Manager to Assign an Owning Player Controller to widgets created by the Manager and Auto Register Default Layers

![*Initialize Extrone UI Manager in Player Controller’s Begin Play*](InitializeUIManager.png)

## Registering Layers

Default Layers specified in the Project Settings will be auto registered when initializing Extrone UI Manager

![*Add Layers that should be registered by default to **Project Settings → Plugins → Extrone UI → Layers → Default Layers***](DefaultLayers.png)

You can also use **[Register UI Layer](../functions/#register-ui-layer)** or **[Register UI Layer Widget](../functions/#register-ui-layer-widget)** functions to register layers

## Creating Screens

Screens that you can push to Layers need to be inhertied from UExtroneScreenBase class

1. Right Click on the Content Browser and select **User Interface** -> **Widget Blueprint**
![Creating Widget Blueprint](CreateNewWidgetBlueprint.png)
2. A new window will appear asking you to select a parent class. Expand the **All Classes** dropdown and search for **ExtroneScreenBase**
![Search for and select ExtroneScreenBase](SearchForExtroneScreenBase.png)
3. Select **ExtroneScreenBase** from the list and click the **Select** Button

The above steps will create a new Widget Blueprint that inherits from UExtroneScreenBase and can be pushed to or popped from layers.

## Pushing Screens

Use **Push Screen to Layer** node to add widgets to layers

![*Pushing Main Menu widget to Main Menu Layer on HUD Begin Play*](PushScreen.png)

## Popping Screens

Use Pop Screen node to remove a widget if its currently the top screen of any layer

![*Use Pop Screen node to remove it if it’s currently the top screen of any layer*](PopScreen.png)