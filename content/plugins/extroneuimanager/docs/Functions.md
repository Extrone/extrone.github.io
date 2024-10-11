---
title: "Function Reference"
summary: Everything you need to know about the functions available in Extrone UI Manager.
url: "/plugins/extrone-ui-manager/documentation/functions"
ShowBreadCrumbs: true
ShowReadingTime: false
ShowWordCount: false
author: " "
cover:
    image: "../../../img/Extrone_UI_Manager_Functions_Thumbnail.png"
    alt: "Extrone UI Manager Plugin Getting Started"
    relative: false
---

# Save Game Object

Let's start by creating a Save Game Object that'll hold all the variables we want to save.

1. Right click on the Content Browser, select Blueprint Class, expand All Classes and search for **SaveGame** and select it.
   ![Alt text](../../img/CreateSaveGame.png)
2. Give it an appropriate name, I called it CustomSaveGame.
   ![Alt text](../../img/CustomSaveGame.png)

You can open it and create all the variables that you want to save.

# Game Instance

Now we need something that manages all the saving and loading. A GameInstance is the perfect place for it since it's persistent from start to end play.

1. Right click on the Content Browser and select Blueprint Class, expand All Classes and search for **GameInstance** and select it.
   ![Alt text](../../img/CreateGameInstance.png)
2. I named it CustomGameInstance.
   ![Alt text](../../img/CustomGameInstance.png)
3. Open it.

## Save and Load

Now wee need to create the functions that'll do the saving and loading.

1. Let's create 2 functions by clicking on the + button in the functions tab, Call them **SaveGame** and **LoadGame**.
   ![Alt text](../../img/Functions_SaveLoad.png)

### SaveGame
Inside the **SaveGame** function, we need to check if there is a Save File that already exists to determine if we need to create a new one or just overwrite it.

1. Right click on the graph and search for **Does Save Game Exist** node and add it the graph.
2. Connect it to the Execution pin, and enter an appropriate name in SlotName, I used "CustomSaveSlot".
   ![Alt text](../../img/SaveGame_DoesSaveSlotExist.png)
3. Now, right click the SaveSlot pin and select Promote to Variable and name it **SaveSlotName**. 
   ![Alt text](../../img/PromoteSlotName.png)
   ![Alt text](../../img/PromoteSlotName1.png)
   This way we won't cause any unwanted issues by misspelling the slot name on other nodes.
4. Add a **Branch** node and connect the **Return Value** of the previous node to it.
5. from false, add the **Create Save Game node** and select the **SaveGame** class we created earlier (In my case CustomSaveGame).

### LoadGame
Now open the LoadGame function. Like the SaveGame function, we need to check if there's already a save file with the slot name so that we either load it if it's available or create one if it's not.

1. Add the **Does Save Game Exist** node and connect it.
2. add a **Branch** and from the false pin call the **SaveGame** function since we need to save the game if doesn't aleady exist.
3. Now add a **Load Game From Slot** node and connect it to the True Pin.
4. connect the **SaveGameRef** variable and the **SaveSlotName** variable to it.