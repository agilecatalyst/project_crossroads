# GAME DESIGN DOCUMENT: CODE NAME "PROJECT CROSSROADS"
## The Ultimate Hyper-Modern Asymmetric RTS (Inspired by Classic C&C 3 / Kane's Wrath)

---

## 1. EXECUTIVE SUMMARY & CORE CONCEPT

### 1.1 The Pitch
**Project Crossroads** is a fast-paced, high-stakes real-time strategy (RTS) game that modernizes the iconic sidebar construction and blistering combat dynamics of *Command & Conquer 3: Tiberium Wars*. Set in an obfuscated, near-future theater echoing the real-world geopolitical clash between Russia and Ukraine (2022–2026), the game pits a massive, brute-force industrial empire against a highly agile, decentralized, tech-forward resistance nation.

### 1.2 Core Pillars
* **Blistering C&C-Style Kineticism:** Ultra-responsive unit micro, instant sidebar queuing, garrisonable urban landscapes, and high-lethality engagements.
* **True Geopolitical Asymmetry:** One faction relies on massed armor, crushing artillery, and traditional forward base building; the other utilizes crowd-funded logistics, decentralized infrastructure, drone networks, and off-map international aid.
* **The Electronic Warfare (EW) Layer:** A revamped Fog of War where information is as valuable as fuel. Jamming GPS, spoofing radar signatures, and maintaining drone reconnaissance dictate battlefield dominance.
* **Territorial Anchor Mechanics:** Traditional mobile Construction Yards (MCVs) are replaced or challenged by static, high-value **Key Regional Cities** that serve as regional production hubs and economic anchors.

---

## 2. THE GEOPOLITICAL FACTIONS

```
========================================================================
                      FACTION COMPARISON MATRIX
========================================================================
Feature              Eurasian Coalition (EAC)    United Borderlands Rep. (UBR)
------------------------------------------------------------------------
Base Philosophy      Centralized Command         Decentralized Resistance
Construction Method  Heavy Armored MCV / Grids   Mobile Rigs & Urban Hubs
Primary Strength     Unstoppable Artillery/Mass  High Mobility, Micro, Drones
Super Weapon         "Zmej" MIRV Satan Silo      "Aegis-Patriot" Interceptor Grid
Reinforcements       On-Map Heavy Factories      Off-Map Safe-Haven Corridors
========================================================================
```

### 2.1 The Eurasian Coalition (EAC) — *Working Title: Russia*
* **Philosophy:** A vast, resource-rich petro-state empire operating on an authoritarian command structure. They rely on overwhelming industrial output, deep legacy reserves of Cold War-era heavy armor, and devastating massed bombardment.
* **Aesthetic:** Brutalist concrete fortresses, thick diesel smoke, heavy cast-iron tracks, and terrifying, exposed rocket-artillery platforms.
* **Unique Faction Mechanics:**
    * *Doctrinal Artillery:* When three or more EAC artillery units fire at the same map grid, it automatically triggers a "Saturation Bombardment," compounding splash damage and instantly collapsing structures.
    * *Slat Armor Upgrades:* EAC vehicles can be upgraded with reactive cage armor, completely mitigating the damage of the first incoming anti-tank guided missile or FPV drone.

### 2.2 The United Borderlands Republic (UBR) — *Working Title: Ukraine*
* **Philosophy:** A fiercely independent coalition of tech-forward border states. Lacking the heavy heavy-industrial footprints of the EAC, they survive through localized defense networks, bleeding-edge autonomous commercial drone adaptations, and international crowd-funding.
* **Aesthetic:** Sleek, improvised, high-tech but scrappy. Camouflaged civilian vehicles retrofitted with anti-tank missiles, modular solar-paneled outposts, and multi-rotor drones.
* **Unique Faction Mechanics:**
    * *Diplomatic Capital Meter:* A real-time tracker of international favor. Filled by protecting civilian assets, uploading drone footage of EAC operations, or completing high-risk secondary objectives. High favor yields massive financial credits and high-tier Western tech shipments.
    * *Decentralized Command:* UBR structures do not require a centralized construction yard. They can unfold hidden "Mobile Support Rigs" in any hidden patch of terrain to expand localized production rings.

### 2.3 The Vanguard Group — *The 3rd Wildcard Faction*
* **Philosophy:** A corporate private military conglomerate operating on international black-market contracts. They do not harvest traditional resources; they secure map zones or urban blocks for neutral AI corporate syndicates in exchange for high-tier currency.
* **Aesthetic:** Slick, unmarked carbon-fiber hulls, autonomous AI ground rovers, and active-camouflage stealth technicals.

---

## 3. CORE GAMEPLAY & MECHANICS

### 3.1 The Economy: Physical Logistics vs. Digital Crowdfunding
The economy utilizes a twin-resource engine:
1.  **Material/Supply Lines (The Physical Resource):** Collected by vulnerable logistics vehicles from raw supply depots or train yards. Used for heavy production and defenses.
2.  **Credits/Crowdfunding (The Digital Resource):** Automatically generated by securing cellular arrays, internet hubs, or through the UBR's Diplomatic Capital Meter. Used for high-tier research and off-map support actions.

### 3.2 The Sidebar UI Design
True to the *C&C 3* layout, the sidebar stands on the right-hand side of the screen with quick-toggle tabs:

```
+-------------------------------------------------------------+
|                         THE SIDEBAR                         |
+-------------------------------------------------------------+
|  [ BUILDINGS ]  |  [ DEFENSES ]  |  [ UNITS ]  |   [ EW ]   |
+-------------------------------------------------------------+
|  [ Power Array ]       [ Grizzly SPAAG ]                    |
|  [ Assembly Hub ]      [ Falcon Strike ]                    |
|  [ Drone Foundry ]     [ FPV Swarm Unit ]                   |
+-------------------------------------------------------------+
| OFF-MAP SUPPORT ACTIONS (Global Cooldowns)                  |
|  [!] Cyber-Jamming Strike (Disables Enemy Minimap)          |
|  [!] Deep-Strike Waypoint Drone Salvo                       |
|  [!] Satan-II Ballistic Multi-Target Launch                 |
+-------------------------------------------------------------+
```

### 3.3 The Electronic Warfare (EW) Layer
* **GPS Jamming Cones:** Heavy EAC mobile trucks can project an active EW field. Inside this field, the UBR player completely loses their minimap, and laser-guided or precision missile strikes miss their marks entirely.
* **Drone Reconnaissance:** UBR players can fill the skies with ultra-cheap, autonomous micro-drones, cutting through the EW fog to expose enemy unit placements, artillery lines, and movement paths.

---

## 4. THE APEX TECH & CRITICAL ASSETS

### 4.1 EAC "Zmej" (Serpent) Satan-II Missile Silo
* **Type:** Tier-4 Superweapon.
* **Mechanic:** Upon countdown completion, the player fires an intercontinental ballistic missile. In mid-air, the missile separates into a **MIRV payload**. The player selects **3 to 5 independent target grids** anywhere on the map. Hypersonic warheads rain down simultaneously, obliterating hardened bases and bypassing mid-tier defenses.

### 4.2 UBR "Aegis-Patriot" Defensive Array
* **Type:** Tier-4 Multi-Structure Defensive Network.
* **Mechanic:** Requires a **Phased-Array Radar Hub** linked to multiple scattered **Long-Range Missile Launcher Batteries**. This system forms an active interception dome over the base. It is the only defense capable of shooting down the EAC's "Zmej" ballistic missiles or heavy tactical bombers. It consumes catastrophic amounts of power, leaving it vulnerable to power-grid sabotage.

### 4.3 UBR "Grizzly" SPAAG (Self-Propelled Anti-Aircraft Gun)
* **Type:** Tier-2 Mobile Counter-Drone Vehicle (Gepard Analogue).
* **Mechanic:** Armed with rapid-fire twin autocannons. Features an active ability: **"Proximity Flak Burst."** When flipped on, it fills the local airspace with programmable air-burst munitions, instantly shredding incoming FPV kamikaze drones and light recon aircraft.

---

## 5. THREE-ACT CAMPAIGN BLUEPRINT

### 5.1 Act I: The Blitzkrieg Blunted
* **Setting:** The opening days of a sudden, overwhelming multi-vector invasion.
* **Core Feature — Key Cities Mechanic:** Traditional mobile construction vehicles (MCVs) are absent for the UBR. Players start in control of **three interconnected Key Regional Cities**. These cities serve as the literal construction yards. If a city falls, that production sector is lost permanently.
* **The Refugee Dilemma:** Civilian vehicles clog the highways. Utilizing heavy equipment to plow through civilian traffic catastrophically damages the *Diplomatic Capital Meter*, locking out late-game international aid. Players must micro infantry squads to clear roads and shepherd refugees while fighting off high-tier EAC armored vanguard elements.

### 5.2 Act II: The War of Attrition & Logistics
* **Setting:** The front lines have locked into a brutal, grinding trench and urban stalemate. 
* **EAC Counter-Strategy — Rail Sabotage & Cyber-Warfare:** The EAC deploys specialized **Spetsnaz Saboteur Infantry** and cyber-strikes. Their goal is to sever the UBR's connection to their **Off-Map Safe Haven Factories** (located in neighboring friendly states).
* **Mechanic:** UBR high-tier weapons (like Western-analogue tanks and aircraft components) are built in untouchable off-map queues using diplomatic credits, then shipped to the front lines via **Strategic Rail Corridors**. EAC players can launch raids to destroy rail junctions or deploy cyber-attacks to freeze the off-map build queues, forcing the UBR into desperate localized defenses.

### 5.3 Act III: The Drone & Precision Revolution
* **Setting:** The technological apex of the war. The UBR unleashes its domestic innovation to push back the occupier.
* **The "Vanguard Falcon" Multi-Role Fighter:** Operating via a **"Strike & Scram"** system. Rather than resting on a vulnerable forward airfield, these jets fly in from off-map via sidebar action, drop laser-guided precision payloads onto heavy EAC artillery clusters, and hit afterburners to escape automated S-400 anti-air envelopes.
* **Custom Long-Range "Tremor" Drones:** Built cheaply inside secured urban city factories. These slow, fragile one-way attack drones possess infinite range. 
* **The Waypoint Mechanic:** The player explicitly draws a **custom flight path line** on the minimap, guiding the drone fleet through blind spots in the EAC's mobile radar coverage. If successful, they strike high-value rear targets like fuel reserves or ammunition dumps, triggering catastrophic, base-wide chain explosions.

---

## 6. KANE'S WRATH INSPIRED SUB-FACTIONS

### 6.1 Eurasian Coalition (EAC) Sub-Factions
* **The Iron Guard (Heavy Armor Focus):** Swaps standard combat units for ultra-heavy armored variants. Features a **"Siegeworks"** upgrade, allowing tanks to physically burrow into the earth, transforming them into heavily fortified, stationary defensive bunkers.
* **The 2nd Artillery Corps (Bombardment Focus):** Unlocks devastating long-range thermobaric systems early. Equipped with automated **"Counter-Battery Radar,"** which automatically orders artillery units to fire back at the origin point of any incoming enemy projectiles.

### 6.2 United Borderlands Republic (UBR) Sub-Factions
* **Aero-Vanguard (Drone Swarm Focus):** Drastically strips back traditional infantry squads in favor of specialized drone operators. Can field massive, high-micro swarms of FPV kamikaze drones and unmanned autonomous ground combat rovers.
* **The Partisan Brigade (Stealth & Ambush Focus):** All infantry and light anti-tank squads (Javelin/NLAW analogues) gain passive invisibility when stationary inside forests, ruins, or tall brush, turning every checkpoint into a lethal kill zone.