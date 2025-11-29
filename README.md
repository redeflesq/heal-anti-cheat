# HealAC — Anti-Cheat Plugin for CS 1.6 (AMXX)

> **A rarity from the old days.**  
Last real update: **2019** — the code was only cleaned and re-released, no modern development continued.

**HealAC** is a lightweight anti-cheat system for Counter-Strike 1.6.  
Tested on a live server for about a year — stable performance, almost no false detections (rarely on SpeedHack).

## Detection & Punishment

| Cheat Type | Action |
|-----------|--------|
| **SpeedHack** | Kick |
| **FastKnife** | Kick |
| **BunnyHop** | Kick **or** Jump Prevention |
| **WallHack / ESP** | Visibility Prevention |

## CVAR Configuration

| Cvar | Default | Description |
|------|---------|-------------|
| `heal_wh_checkevery` | `1` | WallHack check frequency |
| `heal_wh_ignoreteam` | `1` | `0` — block WH even on teammates / `1` — allow WH on teammates |
| `heal_bhop_prevent` | `1` | `0` — kick for BunnyHop / `1` — block jumping |
| `heal_bhop_limit` | `3` | Allowed perfect hops before kick *(only works if prevent=0)* |

> Lightweight and safe to use as an **additional anti-cheat layer**.  
> Practically no performance impact.

## Changelog
### **0.3.5**
- Performance improvements & internal code optimization  
- Removed **SpeedHack toggle cvar** — detection now works automatically  
- Introduced **BunnyHop prevention mode** for cleaner movement validation  

### **0.3.4**
- Fixed a detection inconsistency related to **SpeedHack**  

### **0.3.3**
- Added **BHOP detection** with more consistent jump pattern analysis  

### **0.3.2**
- Added **FastKnife detection**, tracking abnormal swing rates  

### **0.3.1**
- Implemented **SpeedHack detection** for accelerated movement patterns  

### **0.3.0 — Release**
- Added **ESP & WallHack Shield** to block unfair visibility exploits  

## Final Notes

A piece of oldschool CS 1.6 anti-cheat history — still functional, but untouched since 2019.  
Good for classic servers and as a backup layer of protection.
