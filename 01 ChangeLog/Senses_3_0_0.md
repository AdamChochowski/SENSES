# [3.0.0]
### Senses Asset Pack

**Summary:**  
This is one of the largest updates ever released for Senses.  
The amount of internal work, refactoring, and new systems introduced is massive—  
so below you will find **only the biggest and most important highlights**.

---

## 🟢 Added

### **RedHanded System**
A fully modular, rule‑driven framework for handling forbidden areas, illegal interactions, and actions with consequences.  
It consists of four major parts:
- **RedHanded Component** – Core logic that constantly evaluates nearby RedHanded Zones, Objects, and Actions.  
- **RedHanded Zones** – Spatial rule-areas that trigger repercussions based on entering, staying, being detected, or exiting.  
- **RedHanded Objects** – Interactable items whose rules activate on touch, hold, or release events.  - **RedHanded Actions** – Designer-built ScriptableObject actions that can be instant, lasting, abortable, conditional, or global.  

Together these allow you to build stealth gameplay, faction-based logic, security systems, contraband checks, rule violations, and complex interaction consequences with almost no custom code.

---

## 🟢 Added (continued)

### **SceneFaction Manager**
A central system managing scene-wide faction relations, enabling consistent hostility, cooperation, and escalation behaviors across all agents.

### **Live Awareness Debugging**
When Gizmos are enabled, you can now see **live awareness values** directly in the Scene View for easier balancing and debugging.

### **Noise System Expansion**
NoiseComponent now includes an option to emit **Test Noise**, allowing quick debugging without gameplay events.

---

## 🟡 Changed / Improved

### **Documentation – Completely Rewritten**
All documentation was rebuilt **from scratch** for clarity and ease of use:
- Full explanations of every RedHanded subsystem  
- Step-by-step examples  
- New diagrams, tables, and flow explanations  
- Unified terminology across all components  

Additionally, **every Senses and RedHanded component now includes a button at the bottom of the Inspector** that links directly to the **online GitHub documentation** for instant access.

### **Massive Custom Inspector Refresh**
Nearly all inspectors were redesigned:
- Cleaner UI  
- Better grouping  
- Helpful tooltips  
- Consistent structure across all subsystems  
- Faster navigation  

### **Performance & Memory Overhaul**
A huge upgrade to Senses' internal architecture:
- Up to **51% performance increase**
- New memory model using:
  - **Lazy allocation**
  - **Block‑based buffering**
  - **Structure‑of‑Arrays (SoA) pools**
- Significantly lower memory fragmentation
- Higher stability under large AI loads

### **Custom Updater 2.0**
The internal updater now spreads load over multiple frames, giving smoother AI behavior even in large-scale scenes.

---

## 🔵 Fixed

- Fixed **Ignore Rotation X** and several other minor detection issues.
- Numerous small inspector bugs resolved.
- **ScentNodePool** was completely rewritten for stability and faster node iteration.
- Various smaller bugs and inconsistencies across Senses & RedHanded systems.