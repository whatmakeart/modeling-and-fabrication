---
title: "11.03Create Shopbot Tool Fusion 360"
date: 2020-01-26T23:11:13Z
draft: false
---

## Create a Tool Holder 

Create a tool for the 1/4" straight cut router bit. We have other bits in the Fab Studios for cutting out 3D profiles and engraving but you will use the 1/4" bit for most of your cutting. You will create a tool holder and a tool bit. For 2D cutting the tool holder is not needed but you should make it to know the process in case you do any 3D Cutting. For 3D cutting we need to know where the tool holder is and how big it is.  This [video](https://youtu.be/M9MQzYrLhGQ) shows how to create the 1/4" ShopBot Tool. [https://youtu.be/M9MQzYrLhGQ](https://youtu.be/M9MQzYrLhGQ "Share link")

Use the settings and values below to make your tool.

### General Tab

- Description: ER25 Collet Nut
- Vendor: ShopBot
- Product ID: ER25
- Product Link: [https://store.shopbottools.com/products/collet-nut-er25](https://store.shopbottools.com/products/collet-nut-er25)

### Holder Geometry Tab

- Height #1: 17 mm
- Upper Diameter #1: 42 mm
- Lower Diameter #1: 42 mm
- Height #2: 3 mm
- Upper Diameter #2: 42 mm
- Lower Diameter #2: 32 mm

## Create 1/4" Flat End Mill Tool

### Under General Tab

Description: 1/4” Flat Endmill

Vendor: Whiteside

Product ID: 1014

Product Link:

### Cutter Tab

Type: Flat End Mill

Unit: Inches

Clockwise spindle Rotation - yes

Number of Flutes: 2

Material: HSS

### Geometry Tab

- Diameter .25 in
- Shaft Diameter .25 in (fx)
- Overall length: 2.5 in
- Length below Holder: 1.2 in
- Shoulder Length. 1 in
- Flute length: 1 in

### Shaft Tab

Not used for this simple end mill.

### Holder Tab

Not used for 2D and 2.5D cutting but we can select the custom holder we made so we have more visual aid to see if parts are the wrong size in simulation.

### Cutting Data Tab

#### Speeds

- Spindle Speed 18000 rpm
- Surface Speed - Calculated
- Ramp Spindle Speed 18000

#### Feedrates

- Cutting Feedrate 144 in/min
- Feed per tooth - Calculated
- Lead-in Feederate - Calculated
- Lead-out Feedrate - Calculated
- Ramp Feedrate - 72 in/min

#### Vertical Feedrates

- Plunge feedrate 72 in/min
- Feed per revolution - Calculated

#### Passes and Linking

- Use Step-down - check
- Stepdown .125

#### Coolant

- Disabled

<div class="video-grid">

<div class="video-card">

## Create ShopBot Tool Fusion

<div class="iframe-16-9-container" ><iframe class="youTubeIframe" src="https://www.youtube.com/embed/M9MQzYrLhGQ?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>

</div>
