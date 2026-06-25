---
title: "Settings"
summary: Editor Clock Settings can be changed in Editor Preferences -> Editor Clock
url: "/plugins/editorclock/documentation/settings"
draft: true
weight: 200
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
    image: "Editor_Clock_Settings_Thumbnail.png"
    alt: "Editor Clock Plugin Settings"
    relative: false
---

## Settings
Editor Clock Settings can be changed in Editor Preferences -> Editor Clock

### Clock
| Option |  Details |
|:-|:-|
| Time Zone | Select the Time Zone that you want to see the time of <br>Select the empty option at the top to see Local Time|
| Display Format | `EEE` = Short Day of the Week, e.g: Mon	<br>`EEEE` = Full Day of the Week, e.g: Monday	<br>`yy` = Short Year, e.g: 25	<br>`yyyy` = Full Year, e.g: 2025	<br>`M` = Numerical Month, e.g: 3	<br>`MM` = Numerical Month zero padded, e.g: 03	<br>`MMM` = Short Month Name, e.g: Mar	<br>`MMMM` = Full Month Name, e.g: March	<br>`d` = Day of Month, e.g: 8	<br>`dd` = Day of Month zero padded, e.g: 08	<br>`h` = 12 Hour, e.g: 6	<br>`hh` = 12 Hour zero padded, e.g: 06	<br>`HH` = 24 Hour, e.g: 18	<br>`mm` = minutes	<br>`ss` = seconds	<br>`a` = am/pm	<br>`D` = Day of Year	<br>	<br>Disclaimer: 	<br>The order of display of Day Month and Year is controlled by the Editor Locale.	<br>That is, you will get MM/DD/YYYY or DD/MM/YYYY depending on the Editor Locale.	<br>Editor Locale can be changed in Editor Preferences -> Region & Language -> Internationalization -> Editor Locale. |
| Time Offset | Add this amount of offset to current time before displaying. <br>	Can be positive to add time or negative to subtract.<br>	Format is Days.Hours:Minutes:Seconds.Millisecond |

### UI
|Option|Details|
|:-|:-|
|Show Confirmation On|Select Actions that should show a confirmation popup before performing the action|
|Show Notification On|Select when notification should be shown|

### Save
|Option|Details|
|:-|:-|
|Save Data On|Select Actions that should also save clock data after completing the action|

#### Auto Save
|Option|Details|
|:-|:-|
|Auto Save|Enable to automatically save clock data periodically.|
|Auto Save Interval|If Auto Save is Enabled, automatically saves clock data every AutoSaveInterval seconds.|

### Inputs
|Option|Details|
|:-|:-|
|Saved Input Field Values|Input fields whose values should be saved|
|Clear Name Input on Add|Should the Name input field be cleared when a new clock is added|

### Icon Colors
|Option|Details|
|:-|:-|
|Default|Default Color for Icons without dedicated Colors|
|Add|Color for Add Icon|
|Remove|Color for Remove Icon|
|Start|Color for Start Icon|
|Pause|Color for Pause Icon|
|Stop|Color for Stop Icon|
|Reset|Color for Reset Icon|
|Pin|Color for Pin Icon|
|Un Pin|Color for Un Pin Icon|
|Confirm|Color for Confirm Icon|
|Cancel|Color for Cancel Icon|

### Row Colors
|Option|Details|
|:-|:-|
|Even|Background Color for every EVEN Row|
|Odd|Background Color for every ODD Row|

### Background Colors
|Option|Details|
|:-|:-|
|Background 1|Color for Background Layer 1|
|Background 2|Color for Background Layer 2|
|Background 3|Color for Background Layer 3|

### Button Colors
|Option|Details|
|:-|:-|
|Normal|Button Normal Color|
|Hover|Button Hover Color|
|Pressed|Button Press Color|

### Other Colors
|Option|Details|
|:-|:-|
|Separator|Separator Color|

