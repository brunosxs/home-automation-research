# Start

This document is meant to provide guidance for when I start doing home automation, integrating my servers and DVR cctv stuff.
It is meant to guide me for when I decide to start the actual execution of it.

## Overall requirements:

- Proper server integration and usage LOCALLY (no outside access) of my NAS, transcoding server and my containers machine.
- At least 2.5gbps ethernet access between key machines on my network (transcoding, nas, containers, virtualization and main work computer should all have 2.5gbps access between themselves)
- zigbee/thread/matter (tech stack still TBD) server for controlling and getting power consumption from the devices I properly add to my home, NO tuya or proprietary devices as I want full access and management of those to be local.
- Network router is the only thing I am allowing proprietary/closed-garden tech as it is prohibtly expensive to buy compatible routers to create this solution myself at reliable speed. So I will be using DECO from TP-Link for my routers. All because of roaming functionality (which marketing calls mesh network)
- DVR system for at least 8 cameras, recording in x265 or hopefully av1 codec
- Fully integrated home-assistant from which I should be able to manage everything, including looking at camera feeds, charts to examn power consumption and coding home automation.

## What this guide is not:

- Not meant to guide or specify anything related to remote access through internet, this is a whole can of worms that I don´t wanna touch unless I really find real use-cases for me. Even in this situation, the dangers and complexity is not worth for my use case atm.

------------------

----------------------------
| Index                    |
----------------------------
| [DVR software and specs](DVR.md) |
| [Home automation](HomeAutomation.md) |
| [Findings](Findings.md) |