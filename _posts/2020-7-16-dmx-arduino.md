---
layout: post
title: Sending DMX with/over Arduino UNO/MEGA
description: ... intention to control the LED-Bar in my possession ...
image: false
---

<!-- ![photo not found](./img/IMG_5053.jpg) -->
<span class="image right"><img src="{% link assets/images/IMG5053.JPG %}" alt="" /></span>

#### Introduction
This project started with the intention to control the LED-Bar in my possession (ADJ UB 9H) with the hardware available to me. Which is an *Elegoo UNO R3*! BUT to get access into the DMX Protocol, there is an separate IC-Chip needed. Which has to be integrated in the Arduino main circuit as a so called "DMX-Shield". The public-address light industry mostly uses the *MAX485* Chip. In my case I use an *SN75176BP* which has mostly the same structure and did absolute fine for this purpose so far.  
it took me a while to find a working Code Example, I will link it here, after I found it again!

::: tip Interested in an DMX-Protocol INTERFACE?
My research so far suggested that you need to have an **Arduino MEGA 2560** due to its USB-Serial-Port, which is absolute necessary for this kind of connection. *I heard rumors this works with the first ever Arduino UNO Version too*
:::

#### Hardware
* Elegoo UNO R3
* Integrated Circuit: SN75176BP
* DMX or XLR Cable with at least the *female XLR Plug*
* *obviously* DMX-Receiver / Device to Test with

#### Software
* [Arduino IDE](https://www.arduino.cc/en/Main/Software)

#### Code
* Based on this [Code](https://42loop.hfbk-hamburg.de/garage/184)
#### Additional Instructions & Information (external)
* [General Arduino Thread regarding DMX512 with Arduino](https://playground.arduino.cc/Learning/DMX/)
* [Building an DMX Shield with the IC Chip for Arduino](https://playground.arduino.cc/DMX/DMXShield/)
