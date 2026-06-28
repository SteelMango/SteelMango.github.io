---
layout: post
title: "Setting up a £3 L2C Display module"
date: 2026-06-28 10:00:00 -0000
categories: [hardware]
image: /assets/images/liquid_display.jpg
---

![Image of Liquid Display](/assets/images/liquid_display.jpg)

In this post I explain simply how to set up a L2C Display module without soldering and staying to the breadboard/jumperwires, ideal for beginners who own a ESP-32.

## Where I Brought the Screen 
I lied, the screen is actually £3.46 upon editing this post. I was scrolling through Aliexpress for cheap components for my ESP32 and found this, a LCD Display module for £3. Since we don't want to solder, make sure to choose the IIC LCD1602. 

Why a IIC LCD1602?, Because the display module has a little backpack called an ICC. An ICC module helps reduce the amount of wires to connect to the display and additionally allows us to use jumper wires (male to female/female to female). Without the ICC we would need to solder the display module.

[Aliexpress Link](https://www.aliexpress.com/item/1005006100081942.html?invitationCode=NkMweS9YbXd3TjBHbEJTRGFOK1RKaDBmcUFEbmZJVHZNa3VZNlh5bXFhaWVQemFTZUJrNWVWT0s1MU1hdTAyWg&srcSns=sns_Copy&spreadType=socialShare&social_params=61554315384&bizType=ProductDetail&spreadCode=NkMweS9YbXd3TjBHbEJTRGFOK1RKaDBmcUFEbmZJVHZNa3VZNlh5bXFhaWVQemFTZUJrNWVWT0s1MU1hdTAyWg&aff_fcid=d6abd1973f57498cad8784c03e116df7-1782659115028-08384-_EJewm9y&tt=MG&aff_fsk=_EJewm9y&aff_platform=default&sk=_EJewm9y&aff_trace_key=d6abd1973f57498cad8784c03e116df7-1782659115028-08384-_EJewm9y&shareId=61554315384&businessType=ProductDetail&platform=AE&terminal_id=3eb805147cb5464c863135f9e4096156&afSmartRedirect=y)

## Setting up the ESP32 for the Display 

![Pinout diagram of ESP32](/assets/images/pinout_esp32.png)

Now depending on what ESP32 you have, you would need to check out your specifc ESP32 pinout reference. A pinout reference tells you what each pin on the ESP32 does, for example on the ESP32 Devkit v1, the pin "GND" is ground. 
Once you have the display module, if you turn it around and see the little backpack (ICC) I mentione earlier, you'll see four pins. 

1.  GND
2.  VCC
3.  SDA
4.  SCL

If you have a ESP32 Devkit, connect to these pins:
1.  GND = GND
2.  VCC = VIN
3.  SDA = D21
4.  SCL = D22

