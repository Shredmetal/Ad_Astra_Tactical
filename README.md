# Tactical Space Combat Game

## Core Ruleset

### Introduction
This is a technical space combat game where physics, heat management, and component damage determine survival.

### Tech Base
This started as a thought experiment about what space combat would look like. In short - pretty different from atmospheric vehicular actions.

There are several core technologies here and this section is worth reading primarily because it enables you to reason about the effects of your choices, as the rules are essentially a game abstraction of physics limitations.

### Core Technologies

#### Propulsion Technology
Naturally, ships have engines. Currently, we use chemical reactions which have a ton of limitations, including pump cavitation, supersonic flow and low energy density. This could in theory be resolved by:
1. Getting rid of the moving parts
2. Massively increasing energy density

**Fusion Reactors**  
Fusion reactors give us abundant power - crucially, there's a ton of extra energy available for particle accelerators which can enable antimatter production. This means that we can further increase energy density. However, it would not make sense for all ships to use antimatter reactors because there will always be losses in using fusion generated energy to make antimatter. Therefore, antimatter reactors are largely only used in warships.

With all that energy, you can then magnetically accelerate a ferrofluid reaction mass at an extremely high exit velocity. This forms the basis of the propulsion systems of our ships, and how they can pack so much specific impulse for insane accelerations up to 27G, at least for the smallest and fastest ones, frigates.

#### Crew Survival
Unfortunately, humans are not going to survive 27G, we're pretty squishy. A possible solution to this is magnetically doped blood. This means that warship crews have to get their blood magnetically doped so the shipboard anti-G magnetic field can mitigate the effects of acceleration-G by pushing in the opposite direction, supporting human tissues since blood is everywhere. A benefit of this is that we also get artificial gravity.

In terms of the universe here, since magnetic doping might not necessarily be universal, civilian liners do not have artificial gravity and have to do a flip and burn, which is extremely fuel-inefficient.

#### FTL
This is the bit where space magic has to come in - there are no gameplay implications yet but something remotely plausible is preferred. I have chosen Alcubierre drives as the FTL option due to the possibility of interesting scenario packs built around Alcubierre drive based tech like negative space weapons.

#### Weapons Systems

**Lasers**  
Pretty self explanatory since we already have them, but they have to be held on a single spot to burn through a ship's hull to destroy the internal component. Can be entirely negated by the target spinning in place. Of course, when negative laser damage, the target can't shoot back.

**Particle Cannon**  
A weaponised particle accelerator. It fires charged particles at 0.01c. Causes several effects:
1. Kinetic damage
2. Surface superheating of whatever it hits
3. Sub-atomic damage as it strips away various charged particles from the target

Extremely powerful but extremely difficult to hit with, especially at 30 miles against a target that is extremely mobile.

**Missiles**  
Self-explanatory. These will always hit some part of the target, but are very vulnerable to PD (point defence) and are entirely useless until the target's PD has been destroyed.

#### Defensive Systems

**Armour**  
Throughout history, weapons have always beaten armour, and it's the same here. Armour is there entirely as an ablative layer, which is the only reason why lasers don't immediately destroy a component.

**Heat Management**  
Everything a ship does generates heat. However, the ability to store heat is a warship-specific capability for stealth. Without a heat signature and advanced low-observable technology, it is impossible to detect a warship in the vastness of space. Heat banks have a limit though, and they will need to be vented eventually. Failure to do so can cause complete destruction of a ship.

With that, the effects of all your decisions and why good or bad things happen should make logical sense.

### Components Needed To Play
- D20 dice (at least 2 per player)
- D6 dice (at least 2 per player)
- 8 ship miniatures (4 per side)
- 8 Heat tracking markers/dials (0-40 range)
- System status cards for each ship
- Range rulers (30" minimum, 40" measuring tape recommended)

### Game Setup
- Each player deploys 4 frigates
- Each ship starts with:
  - 0 heat
  - All systems functional
  - 4 missiles
  - Full movement capability

### Ship Systems
Each ship tracks six critical components:
- Engine (Destruction = Ship Lost)
- Magnetic Field (Damage = 9G limit)
- Fire Control (Damage = Hit penalties)
- Heat Management (Damage = No heat storage)
- Missile Bays (Damage = Lose missiles)
- Point Defense (Damage = Missile vulnerable)

### Turn Sequence
Each game turn consists of five phases, executed in order:

#### 1. Heat Management Phase

**Heat Management System**
- Add heat from previous turn's actions
- Each ship must choose:
  - Store heat (remain stealthy, standard hit receiving chance)
  - Vent heat (visible to thermals, if also visible to visual, attack rolls get a +1 bonus against you) - vents 10 heat per turn

**Critical Heat Threshold**: 30
- Going over causes 1/3 damage to the heat management system
- 3 crits to destruction
- Crits can only be caused by overheating
- Remain in this state for 3 turns and your heat management system explodes, but technically, the heat cap is unlimited while you still have the system

**Destroyed Heat Management System Effects**:
- No storage, must continuously vent
- Death caused if heat generated cannot be vented or stored
- Example: Firing particle cannon (8 heat) and moving 25-27G (5 heat) with destroyed heat management in one turn (13 heat total) causes explosion

#### 2. Movement Phase
- Ships move in initiative order, roll for initiative each turn
- High initiative moves ships first, low initiative moves second

**Movement Capabilities**:
- Frigates: Up to 27G with functioning magnetic system
- 2D Movement - 3D is a bit hard on a tabletop
- Declare G-forces before moving

**Heat Generation Table**:
| G-Force  | Heat Generated |
|----------|---------------|
| 1-4G 	| 1 heat   	|
| 5-9G 	| 2 heat   	|
| 10-18G   | 3 heat   	|
| 19-24G   | 4 heat   	|
| 25-27G   | 5 heat   	|

**G-Force Hit Receiving Modifications**:
| G-Force  | Roll Modification |
|----------|------------------|
| 1-4G 	| + 2         	|
| 5-9G 	| + 1         	|
| 10-18G   | + 0         	|
| 19-24G   | - 1         	|
| 25-27G   | - 2         	|

**G-Force Movement Rules**:
- Base movement: 1" per G
- Maximum normal: 24G (24")
- Maximum damaged: 9G (9")

**Movement Restrictions**:
- Must declare G-force before moving
- Cannot exceed maximum G based on system status
- All movement must be in straight lines
- Can make one course adjustment per move

#### 3. Detection Phase
Check each ship's visibility:
- Venting heat = Automatically detected
- Visual range ~30 miles (30" on table)
- Heat signatures reveal position
- Detected ships can be targeted but only by the ship that can detect it
- Targeting information cannot be shared unless using squadron tactics
- Ships venting and in visual range give attackers +1 roll bonus to hit

#### 4. Combat Phase
High initiative shoots AND RESOLVES DAMAGE IMMEDIATELY first.

Each ship can use one weapon system per turn:

**Laser System**:
- Costs 4 heat
- Always guaranteed hit
- Roll d6 for hit location
- Requires 2 consecutive hits on same location for damage
- Defender can choose to evade:
  - Declare before hit location roll but AFTER attacker declares laser firing
  - Loses their next shooting action
  - Negates the hit entirely

**Particle Cannon**:
- Costs 8 heat
- Range requirements:
  - Long Range: roll at least 39 using 2d20, then roll d6 for hit location
  - Mid Range: roll at least

**Particle Cannon** (continued):
- Range requirements:
  - Long Range: roll at least 39 using 2d20, then roll d6 for hit location
  - Mid Range: roll at least 34 using 2d20, then roll d6 for hit location
  - Close Range: Guaranteed hit, roll d6 for hit location
- Hit immediately kills component
- No defence possible

**Missile System**:
- Each ship starts with 4 missiles
- Can only target ships with destroyed PD
- 66.6% chance to hit (roll 3+ on d6)
- Destroys random component on hit (roll d6 for component)
- Unable to use if missile bays destroyed

#### 5. System Status Phase
- Check component damage on all ships
- Resolve system effects
- Update ship status cards

### Damage Resolution

#### Component Damage Effects

**Engine**:
- If destroyed: Ship is lost
- No partial damage

**Magnetic Field Generator**:
- If destroyed: Maximum 9G movement
- Increases vulnerability to high-G maneuvers
- Able to G-Force Override:
  - Declaration: Start of movement
  - Risk: Crew blackout
  - Roll: Based on G-force
  - Failure: Ship helpless

**GLOC Table**:
| G-Force  | Required Roll |
|----------|--------------|
| 10-15G   | 15+ on d20   |
| 16-20G   | 17+ on d20   |
| 21-24G   | 19+ on d20   |
| 25-27G   | Natural 20   |

*GLOC Effects*:
- No actions for turn (no movement, cannot react)
- +3 hit receiving rolls
- If success, standard hit receive chance penalty does not apply for one turn

**Fire Control**:
If destroyed:
- Lasers must now roll 5+ on a d6 to hit
- -2 to particle cannon rolls
- -2 to missile hit rolls

**Heat Management**:
If destroyed:
- Cannot store heat at all
- Must continuously vent

If heat > 30:
- Add one crit to that ship's heat management system

**Missile Bays**:
If destroyed:
- Lose all remaining missiles
- Cannot launch missiles

**Point Defense**:
If destroyed:
- Ship becomes vulnerable to missiles
- No defense against incoming missiles

#### Hit Location
- Roll d6 for location
- Record damage on ship status card
- Apply effects immediately

### Combat Details

#### Range Bands
- Close Range: 0-8"
- Mid Range: 8-25"
- Long Range: 25-40"
- Beyond 30": Only thermal detection possible

### Squadron Rules

#### Formation Types

**1. Defensive Sphere**
- Requirement: All ships within 9" of centre
- Benefit: Share PD Coverage, if ship has lost PD, being in sphere with at least one ship having PD extends missile invulnerability to other ship
- Drawback: PD can be overwhelmed. Each PD system can only destroy 2 missiles. If the squadron has only 2 ships and 1 PD system between them, if 4 enemy ships each launch a missile, the defending squadron is guaranteed to receive two component hits.

**2. Attack Line**
- Requirement: Ships in linear formation 6" apart
- Benefit: Combined targeting data (+1 per ship in line to all hit rolls)
- Drawback: Enemies receive +1 to all hit rolls when flanking the line

**3. Screening**
- Requirement: Two ships forward of ship or ships being screened, max 9" apart
- Benefit: Forward ships can mask heat signatures of rear ships (i.e. rear ships can vent without being detected thermally) and share targeting data with rear ships
- Drawback: Forward ships can be shot at by enemies outside of even long range of the rear ships

**4. Dispersed**
- Requirement: No ships within 9" of each other
- Benefit: If two ships attack a single target from opposing directions, both ships get a +2 to hit rolls
- Drawback: No mutual support

### Victory Conditions
- Destroy all enemy ships
- [Further development possible here]

