# FeedBack-Reactive.vip
Free, external. Undetected and tested in comp, (not rage tested in prem only legit) this is version 0.1. I have rewritten a new hit chance not just pasted it so it's a bit touchy. Please Please send feedback or bugs back etc

# YES, Reactive has a built in sdk dumper and viewer. Perfect to pair with a coding project or just dead and want to look through the internals of cs2.
Preview

<img width="1920" height="1080" alt="menu_1790265390637" src="https://github.com/user-attachments/assets/a1947952-62d9-4331-8944-66cc6f32e7ab" />

Encourage people to write their own little esp. external or internal.   

I'm studying software engineering and development, this is a side project to help learn more about c++, mechanics, vectors, angles, and RE/Detection vectors and bypasses :) 

So thought I'd share and ask for constructive feedback :) 

Preview!
<img width="1920" height="1200" alt="menu_1790258096055" src="https://github.com/user-attachments/assets/fb996780-e110-4905-b5f0-091750ecd2f7" />
<img width="1920" height="1200" alt="menu_1790251074739" src="https://github.com/user-attachments/assets/bc1fbee7-684c-4ccb-a114-89244f49d913" />
<img width="1920" height="1200" alt="menu_1790258048049" src="https://github.com/user-attachments/assets/846f16d8-e253-4146-8800-69d4f11a0084" />



Known bugs, 
- Visuals can break at times, I'm still optimizing, they are lightweight cpu visuals. Should run on any pc without gpu/low graphics
- Trigger hit-chance is a bit funky, it's self-made and is calculated via valves RNG Seeds pre weapon something I've been experimenting with
- Third Person isn't fully implemented. just a placeholder as a reminder to me to do it.  
- FOV changer, works, but has a little bug on reload. again, focused too much on trigger. Might also cause laggy visuals as I haven't optimized the FOV change. 
- Not much else really. Min damage in aim has just been made so might be abit buggy with picking shots that meet the required hit chance. That i can think of at this time.
- SKINS DO NOT WORK YET, external skins are hard to do, especially when not pasting some old out of dated pasted src. So, give me some time :)
- WORLD MONIPULATION, I started and then pivoted back to hit-chance seed trigger logic. This is not yet implemented logic wise it's just ready for me to start writing out. 

Again 0.1

This is being designed as a undetectable (Don't complain if vac flags you but I have tested thoroughly with all styles of game play legit, semi, rage in comp. non-prime and prime. so i can say 98% in comp you are fine to do anything, idk about prem raging though be warned)

Don't have a driver so don't except it to bypass faceit but i haven't tried.. 

### Features

- **Combat**
  - **Aimbot**: Master toggle, bindable key (`Hold` / `Toggle` / `Always On`), Team Check, Visibility Check
    - *Bones*: Head, Neck, Chest, Stomach, Arms, Legs, Nearest Bone
    - *Priority*: Closest to Crosshair, Distance, Lowest HP, Most Lost HP
    - *Targeting*: FOV (0.01°–180°), 360° Omni Mode, Large-FOV Snap Assist, FOV Circle Overlay
    - *Control*: Smoothing (1.0–30.0+), Min Damage Gate, Standalone RCS (Pitch/Yaw 0–2.0x)
  - **Humanization**: Trajectory Curves (`Log-Normal`, `Min-Jerk`, `Bézier / Wrist Arc`, `Adaptive Power`)
    - *Dynamics*: Wrist Arc Scale, Curve Exponent, Neuromuscular Ramp, Ballistic Submovements
    - *Noise*: Micro-Jitter, Resonant Tremor (6–12 Hz, Amplitude)
  - **Triggerbot**: Dedicated 1 kHz loop, bindable key, Reaction Delay (0–300 ms), Hold Duration
    - *Targeting*: Hitbox Shrink Scale (0.50–1.00), Hitbox Mask (Head–Legs), Min Damage Gate, Auto-Scope, FFA Mode
    - *SeedSync Engine*: Live Valve SHA-1 Spread Sync, Require Current Seed (Live Seed Lock), Hitchance (0–100%), Bucket Guard, Local Origin Lead
  - **Semi-Rage / AutoWall**: Multi-surface penetration simulation, Min Damage (1–100 HP), Auto-Shoot, Independent Wall Hitchance, Wall Seed Lock

- **Visuals**
  - **Player ESP**: Multi-Core SIMD pipeline, Team Check, Visibility Check
    - *Boxes*: 2D Boxes (Normal / Corner / Translucent Fill), Pose-Aware Box Fitting
    - *Overlays*: Skeletons, Head Dot, Health Bar + Exact HP, Armor Text, Player Names, Weapon Text, Distance, Snaplines (Bottom/Crosshair/Top)
  - **Bullet Tracers**: 3D Ballistic Lines (Local / Enemy), Custom Colors, Duration (0.5–5.0s)
  - **Chams**: Dual-Path GPU/CPU Skinned Mesh, Wireframe, Rainbow/Hue Cycle
    - *Shaders (31 Materials)*: Solid, Shaded, Metallic, Latex, Glow/Fresnel, Glass, Galaxy, Opal, Aurora, Obsidian, Crystal, Enamel, Oil Slick, Carbon, Marble, Lava
    - *Layering*: Pattern, Rim, Glow, Outline (Independent Color, Opacity, Scale, Speed) + 8 Presets
  - **World Indicators**: Planted C4 ESP (Site, Defuse Bar, Countdown), LoS State Dot, Spectator List (Names / Local Only)

- **Movement**
  - **Bunny Hop**: Automatic ground-synchronized hop 
  - **Predictive Auto-Stop**: Automatic counter-strafing (`Early Stop`, `On-Shot`, `Between-Shots`)

- **World & Camera**
  - **Atmosphere**: Presets (`Neutral`, `Night`, `Dark`, `Clear Fog`, `Dusk`), Intensity, Transition Speed, Fog Override, Sky/Light Dimming, Post-Processing
  - **Camera**: Custom FOV Slider (60°–140°)

- **Skins**
  - **Weapon Changer**: AK-47, M4A4, M4A1-S, AWP, Deagle, USP-S, Glock-18
  - *Attributes*: Paint Kit ID, Wear (0.0001–0.9999), Seed, StatTrak + Kills, Name Tag, Quick-Draw (Q-Q)

- **HUDs & Diagnostics**
  - **Telemetry HUD**: Live HS%, Accuracy%, ADR, Anti-Flag Warning Alerts (HS%, Accuracy, Pre-fire)
  - **Trigger Log HUD**: Live shot dispatch, seed status, and rejection logger

- **System & Security**
  - **Streamproof**: Hardware-level screen capture exclusion (`WDA_EXCLUDEFROMCAPTURE`)
  - **Profiles**: 34 Per-Weapon Profiles (Global Override toggle), Config Manager (`Save`, `Load`, `Save As`, `Delete`, `Defaults`)
  - **UI Engine**: Custom RGBA Theme Picker, VSync Toggle, FPS Counter, Watermark, Console Test Bench, Schema/Netvar Browser

---

## Future Plans

- [Auto strafer.] 
- [FOV bug catching + visual optimization] 
- [World manipulation] 
- [ETC (it's to early to think ahead (time wise im tired will update hahaha]
