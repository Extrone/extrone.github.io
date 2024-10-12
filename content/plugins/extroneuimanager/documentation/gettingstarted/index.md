---
title: "Getting Started"
summary: Everything you need to know to start using the plugin.
url: "/plugins/extrone-ui-manager/documentation/getting-started"
weight: 1
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
Tags: ["Extrone UI Manager", "UE 5.4"]
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

## Pushing Screens

Use **Push Screen to Layer** node to add widgets to layers

![*Pushing Main Menu widget to Main Menu Layer on HUD Begin Play*](PushScreen.png)

## Popping Screens

Use Pop Screen node to remove a widget if its currently the top screen of any layer

![*Use Pop Screen node to remove it if it’s currently the top screen of any layer*](PopScreen.png)