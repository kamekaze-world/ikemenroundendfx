# IKEMEN GO Universal Round Transition System 1.1 By Kamekaze 
## 6/23/2024
**Mail** - ilive@kamekaze.world

**Twitter** - @OldEra_Kamekaze

**Bsky** - kamekaze.world

**Fgc network** - Kamekaze@fgc.network

### FOR IKEMEN GO .99 OR LATER ONLY

## Change History
### 1.1:
Roundnotover not being respected fixed.

## Description
This code allows you to create a custom round end and round start
animation as zss code. The functions below give you total control of the transitions
either the round end or round start. They are the only things you should directly
modify other than the fight.def and transition time values specified below.

The **"IKT"** refers to the fx the transition uses by default under 
**"ik_roundtransition"** def, air, sff and snd files. The ik_roundtransition.def must be added to your
commonFX area of the config file and this file must be added to your CommonStates area of your config file.

The values within the roundtransition.zss **MUST** match the values in the fight.def as long as we cannot see the values in engine. EG.

```
map(over_time):=270;
map(over_waittime):=45;
map(over_wintime):=45;

values from fight.def
over.time = 270 
over.wintime = 45 
over.waittime = 45 
```

## Instructions

For the round end transition effect, you must define the total time the transition effect will take to complete, the value is labled as:
``root,map(transition_time):=80;``

Once your time is defined, you can put your transition code in the roundstartfx or roundendfx functions provided. There is example code there in [ZSS](https://github.com/ikemen-engine/Ikemen-GO/wiki/ZSS) 
is entirely customizeable. There is a working example provided in the code itself.
