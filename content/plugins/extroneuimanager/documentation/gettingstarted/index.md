---
title: "Getting Started"
summary: Everything you need to know to start using the plugin.
url: "/plugins/extrone-ui-manager/documentation/getting-started"
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
ShowToc: true
author: " "
cover:
    image: "../../../img/Extrone_UI_Manager_GettingStarted_Thumbnail.png"
    alt: "Extrone UI Manager Plugin Getting Started"
    relative: false
---

## Installing the Plugin

1. Open Epic Games Launcher and navigate to **Unreal Engine → Library → Vault**
2. Search for Extrone UI Manager
3. Click Install to Engine and select your preferred engine version
4. Wait for the plugin to be downloaded and installed
5. Open your project and navigate to **Edit → Plugins**
6. Search for Extrone UI Manager
7. Enable Extrone UI Manager and Restart the Editor

## Initializing UI Manager Subsystem

<aside>
<img src="/icons/layers_gray.svg" alt="/icons/layers_gray.svg" width="40px" />

Initialize Extrone UI Manager to Assign an Owning Player Controller to widgets created by the Manager and Auto Register Default Layers

</aside>

![*Initialize Extrone UI Manager in Player Controller’s Begin Play*](InitializeUIManager.png)

*Initialize Extrone UI Manager in Player Controller’s Begin Play*

## Registering Layers

<aside>
<img src="/icons/layers_gray.svg" alt="/icons/layers_gray.svg" width="40px" />

Default Layers specified in the Project Settings will be auto registered when initializing Extrone UI Manager

</aside>

![*Add Layers that should be registered by default to **Project Settings → Plugins → Extrone UI → Layers → Default Layers***](DefaultLayers.png)

*Add Layers that should be registered by default to **Project Settings → Plugins → Extrone UI → Layers → Default Layers***

## Pushing Screens

<aside>
<img src="/icons/layers_gray.svg" alt="/icons/layers_gray.svg" width="40px" />

Use **Push Screen to Layer** node to add widgets to layers

</aside>

![*Pushing Main Menu widget to Main Menu Layer on HUD Begin Play*](PushScreen.png)

*Pushing Main Menu widget to Main Menu Layer on HUD Begin Play*

## Popping Screens

<aside>
<img src="/icons/layers_gray.svg" alt="/icons/layers_gray.svg" width="40px" />

Use Pop Screen node to remove a widget if its currently the top screen of any layer

</aside>

![*Use Pop Screen node to remove it if it’s currently the top screen of any layer*](PopScreen.png)

*Use Pop Screen node to remove it if it’s currently the top screen of any layer*