# Journal: Day 1 – 15 Oct 2026: Research, Scoping & Concept Planning

**Time spent:** ~6 hours

### What I Did
- Researched LED diffusion techniques in 3D printing to figure out how to completely eliminate visible LED "hotspots" (decided on a 3 mm wall thickness with translucent white PETG and an internal reflective core)
- Compared WS2812B LED strip densities (chose 60 LEDs/m for smoother color blending and gradients)
- Sketched out initial design concepts for a modern geometric pillar enclosure in Fusion 360
- Drafted the base ESPHome YAML configuration for the WS2812B strip and planned out GPIO pin assignments on the ESP32

<img width="960" height="960" alt="image" src="https://github.com/user-attachments/assets/bbae0e38-edc4-4ea4-94aa-2237cb67d6f4" />

### Design Decisions
| Decision | Why |
|---|---|
| **Translucent white PETG** | Offers great layer adhesion and durability while scattering light evenly compared to standard opaque PLA |
| **60 LEDs/m density** | Provides enough resolution for fluid animations without overloading power draw |
| **ESP32 microcontroller** | Enables direct local integration with Home Assistant over Wi-Fi without needing extra bridge hardware |

### Problems
- High-density LED strips draw significant current at full white brightness; planning for proper 5V power distribution is essential to prevent voltage drop and color shifting.
- Learned about light scattering physics in 3D-printed translucent materials to optimize shell wall thickness.

### Next Steps
- [ ] Calculate exact strip length and power supply amperage requirements based on final physical dimensions
- [ ] Test different infill patterns in slicer software to see how they impact light transmission
- [ ] Model the main geometric outer shell and internal LED spine in Fusion 360
- [ ] Test-flash the initial ESPHome light configuration on an ESP32 bench setup
