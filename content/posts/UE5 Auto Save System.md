---
title: "Create an Auto Save System in Unreal Engine"
summary: "Learn how to quickly create an Auto Save System in Unreal Engine 4 or 5"
date: 2023-07-07T17:50:00+05:30
draft: true
cover:
    image: "../../img/AutoSaveSystem.png"
    alt: "Inventory"
    relative: false

tags:
    - Development
    - Go
    - fast
    - Blogging

ShowToc: true
ShowPostNavLinks: true
---

# Save Game Object

Let's start by creating a Save Game Object that'll hold all the variables we want to save.

- Right click on the Content Browser, select **Blueprint Class**, expand **All Classes** and search for **SaveGame** and select it.
   ![Alt text](../../img/CreateSaveGame.png)
- Give it an appropriate name, I called it CustomSaveGame.
   ![Alt text](../../img/CustomSaveGame.png)

You can open it and create all the variables that you want to save.

# Game Instance

Now we need something that manages all the saving and loading. A GameInstance is the perfect place for it since it's persistent from start to end play.

- Right click on the Content Browser and select Blueprint Class, expand All Classes and search for GameInstance and select it.
   ![Alt text](../../img/CreateGameInstance.png)
- I named it CustomGameInstance.
   ![Alt text](../../img/CustomGameInstance.png)
- Open it.

## Save and Load

Now wee need to create the functions that'll do the saving and loading.

- Let's create 2 functions by clicking on the + button in the functions tab, Call them SaveGame and LoadGame.
 ![Alt text](../../img/Functions_SaveLoad.png)

Inside the SaveGame function, we need to check if there is a Save File that already exists to determine if we need to create a new one or just overwrite it.

- Right click on the graph and search for Does Save Game Exist node and add it the graph.
- Connect it to the Execution pin, and enter an appropriate name in SlotName, I used "CustomSaveSlot".
  ![Alt text](../../img/SaveGame_DoesSaveSlotExist.png)
- Now, right click the SaveSlot pin and select Promote to Variable and name it SaveSlotName. 
  ![Alt text](../../img/PromoteSlotName.png)
  ![Alt text](../../img/PromoteSlotName1.png)
  This way we won't cause any unwanted issues by misspelling the slot name on other nodes.