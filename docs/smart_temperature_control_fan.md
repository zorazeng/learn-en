
## Goal
---

- Make a smart temperature control fan. 

## Materials
---
- 1 x [Smarthome kit](https://www.elecfreaks.com/estore)
- 1 x corrugated board
- 2 x small sticks
- 1 x glue

## Background
---  
###Meaning of smart temperature control fan

- The smart temperature control fan is a created product base on smart home.That's say, science come from life.

### What is smart temperature control fan
- The room will at high temperature when temperature degree is higher than 30° and make people feel uncomfortable.The temperature sensor will send this signal to micro:bit，and micro:bit send this signal to the fan. Then, the fan will drive until the degree of room under 30° to keeping room at comfortable temperature.

![](https://i.imgur.com/06g0wlF.png)

## Practical operation
---
Materials: corrugated board and cutter

![](https://i.imgur.com/PuJE7uj.jpg)

Build as below picture：

![](https://i.imgur.com/5sc9bid.jpg)

Side

![](https://i.imgur.com/hvnmUhO.jpg)

Paste devices as below piture:

![](https://i.imgur.com/C1lu2Vz.jpg)

## Hardware connect
---

![](https://i.imgur.com/hkOaYEu.png)

## Software
---
[makecode](https://makecode.microbit.org/#)

[Edge Connector Data Sheet](https://www.elecfreaks.com/learn-cn/Edge_Connector_Data_Sheet/)

## Programming
---
### Step 1

Go to MakeCode page, click Advanced in the code block and click on Extensions.

![](https://i.imgur.com/2qCyzQ7.png)

We need to add a new codebase for programming of smart home. Finding “Add Package” in the bottom of code block and click it. Then a message box will show up, search “smart home"， and download this new codebase.

![](https://i.imgur.com/QR2s7LD.png)

Note：If there is a hint says some codebase will be deleted because of incompatibility. Don't worry. You could go ahead as the hint or build a new item in item menu bar.

### Step 2
Drag on start block from Basic and drag initialize OLED block from OLED, change height to 64, width to 128.

![](https://i.imgur.com/NSOCUxe.png)

Drag forever block from Basic, add temp variables in Variable, then drag set item to snap into forever, change item to temp and drag value of temperature behind it. Change value of temperature to ℃ and at pin to P1. 

![](https://i.imgur.com/wPfZA5F.png)

### Step 3

Now let's start OLED code.

Drag clear OLED display under set temp to. Then,drag show (without newline) string ‘Temperature’ under clear OLED display. Last, drag show(without newline) number temp."Without newline" is for newline displaying string and temperature value.

![](https://i.imgur.com/gZwzVGd.png)

### Step 4

Our goal is using micro:bit driving the fan when the value of temperature is higher than 30°, so temp>30 is a judgement condition. In that way, we need drag "if else" from Logic, set temp>30. 

![](https://i.imgur.com/Ys6Hcm3.png)

### Step 5

We add start melody repeating under if ,set melody to ba ding and repeat once，micro:bit will send signal to fan through P2. Then set fan works 5 seconds and stops 5 seconds. The temperature sensor judge whether go loop by gotting the temperature degree. Else means if above condistion were false, the fan will keep rest. 

![](https://i.imgur.com/FHAWwTm.png)

### Programming


Make code：[https://makecode.microbit.org/_AqMEtEbUtPTE](https://makecode.microbit.org/_AqMEtEbUtPTE)

You also could directly download program visit website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_AqMEtEbUtPTE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

## Result
---
When temperature degree is higher than 30°, buzzer "ba ding" , fan driving to keep room comfortable.

![](https://i.imgur.com/mv5oVws.jpg)

When temperature degree is less than 30°，the fan will automatically stop, and the room at comfortable temperature.

![](https://i.imgur.com/Rtptdzw.jpg)

## Think
---
How to adjust speed of fan to control cooling rate in the room. 


## Questions
---


## More information   
---
