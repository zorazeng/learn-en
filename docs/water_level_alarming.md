
## Goal
---

- Make a water level alarming.

## Materials
---

- 1 x [Smarthome kit](https://www.elecfreaks.com/estore)
- 1 x tank

## Background
---
### What is water level alarming 
- We can't live without water, but much water will cause flood. Water level alarming can detect water level, micro:bit will received signals when the water level over security line and control lift pump to pumping.

### Water level alarming operation
- When micro：bit received signal of soil moisture sensor,relay will drive and supply power to lift pump for pumping redundant water.

![](https://i.imgur.com/OsjzuWx.png)

## Practical operation
---
Preparing a tank and paste devices as below piture:

![](https://i.imgur.com/86tb1yO.jpg)

## Hardware connect
---

![](https://i.imgur.com/LRBAV68.png)





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

Snap if statement into forever,set analog read pin P2 > 500, that's say when P2 > 500, the water level is higher than security line.

![](https://i.imgur.com/xa3pCF4.png)

### Step 3

Set start melody "ba ding" repeating once as alarming voice, set digital write pin P1 to 1 as driving the pumping.

![](https://i.imgur.com/zhdgMcI.png)

### Step 4
Else，set digital write pin P1 to 0 as turning off the pump.

![](https://i.imgur.com/lfQVbVh.png)

### Programming

Make code：[https://makecode.microbit.org/_1XpJDo2Y0aDL](https://makecode.microbit.org/_1XpJDo2Y0aDL)

You also could directly download program visit website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_1XpJDo2Y0aDL" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---

## Result
---
When the water level over security line,micro:bit will control lift pump to pumping.

Pumping:

![](https://i.imgur.com/991WoLx.jpg)

Stop pumping:

![](https://i.imgur.com/hPf3xtQ.jpg)

## Think
---
How to use micro:bit control water level in fish tank ?

## Questions
---


## More information  
---

