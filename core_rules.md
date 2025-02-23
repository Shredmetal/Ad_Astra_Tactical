### Components Needed To Play
- D20 dice (at least 2 per player)
- D6 dice (at least 2 per player)
- Ship miniatures (Anything roughly ship-shaped and about 2 inches in length)
- Heat tracking markers/dials (equal number to ship miniatures) (0-40 range)
- System status cards for each ship
- Range rulers (30" minimum, 40" measuring tape recommended)

### Game Setup
- Each player deploys their ships on opposite sides of the table
- Each ship starts with:
  - 0 heat
  - All systems functional
  - 4 missiles
  - Full movement capability
- Deployment zones are opposite table edges, up to 6" in from the edge
- Minimum starting distance between opposing forces: 24"

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
  - Store heat (remain stealthy, invisible to thermals, standard hit receiving chance)
  - Radiate heat (visible to thermals, if also visible to visual, attack rolls get a +1 bonus against you) - radiates 10 heat per turn

**Critical Heat Threshold**: 30
- Going over causes 1/3 damage to the heat management system
- 3 crits to destruction
- Crits can only be caused by overheating
- Remain in this state for 3 turns and your heat management system explodes, exceeding 30 just causes damage but allows continued heat accumulation

**Destroyed Heat Management System Effects**:
- No storage, must continuously radiate
- Death caused if heat generated cannot be radiated or stored
- Example: Firing particle cannon (8 heat) and moving 25-27G (5 heat) with destroyed heat management in one turn (13 heat total) causes explosion

#### 2. Movement Phase
- Ships move in initiative order, roll for initiative each turn
- High initiative moves ships first, low initiative moves second

**Movement Capabilities**:
- Frigates: Up to 27G with functioning magnetic system (other classes to be added in the future)
- 2D Movement - 3D is a bit hard on a tabletop
- Declare G-forces before moving
- You can point and burn in any direction and move in any direction in a straight line
- You can point in any direction after moving

**Heat Generation Table**:

| G-Force | Heat Generated |
|---------|----------------|
| 1-4G 	  | 1 heat   	     |
| 5-9G 	  | 2 heat   	     |
| 10-18G  | 3 heat   	     |
| 19-24G  | 4 heat   	     |
| 25-27G  | 5 heat   	     |

**G-Force Hit Receiving Modifications**:

| G-Force | Roll Modification |
|---------|-------------------|
| 1-4G 	  | + 2         	     |
| 5-9G 	  | + 1         	     |
| 10-18G  | + 0         	     |
| 19-24G  | - 1         	     |
| 25-27G  | - 2         	     |

**G-Force Movement Rules**:
- Base movement: 1" per G

**Movement Restrictions**:
- Must declare G-force before moving
- Cannot exceed maximum G based on system status
- All movement must be in straight lines
- Can make one course adjustment per move

#### 3. Detection Phase

Check each ship's visibility:
- Radiating heat = Automatically detected
- Visual range ~30 miles (30" on table)
- Heat signatures reveal position
- Detected ships can be targeted but only by the ship that can detect it
- Targeting information cannot be shared unless using squadron tactics
- Ships radiating and in visual range give attackers +1 roll bonus to hit

#### 4. Combat Phase

1. High initiative player selects ship to fire
2. Resolve weapon effects and damage immediately
3. Low initiative player selects ship to fire
4. Continue alternating until all ships have fired or passed

Each ship can use one weapon system per turn:

**Laser System**:
- Costs 4 heat
- Always guaranteed hit
- Roll d6 for hit location for first shot
- Subsequent laser shots from the same attacking ship or another attacking ship require a 5+ roll from a d6 and it will take out the same component, if this second roll fails, the attacker rolls a d6 again to determine where the laser hit
- Requires 2 consecutive hits on same location for damage
- Defender can choose to evade:
  - Declare before hit location roll but AFTER attacker declares laser firing
  - Loses their next shooting action
  - Negates the hit entirely
  - Evasion is a 1-9G burn in any direction, with the attendant low-G movement penalties and movement heat buildup

**Particle Cannon**:
- Costs 8 heat
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
- Max range of 20" because your missile needs to constantly burn reaction mass to manoeuvre in space
- Destroys random component on hit (roll d6 for component)
- Unable to use if missile bays destroyed

#### 5. System Status Phase

- Check component damage on all ships
- Resolve system effects
- Update ship status cards

### Damage Resolution

#### Component Damage Effects

#### Hit Location Table
| D6 Roll | Component Hit   |
|---------|-----------------|
| 1       | Engine          |
| 2       | Magnetic Field  |
| 3       | Fire Control    |
| 4       | Heat Management |
| 5       | Missile Bays    |
| 6       | Point Defense   |

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

| G-Force | Required Roll |
|---------|---------------|
| 10-15G  | 15+ on d20    |
| 16-20G  | 17+ on d20    |
| 21-24G  | 19+ on d20    |
| 25-27G  | Natural 20    |

*GLOC Effects*:
- No actions for turn (no movement, cannot react)
- +3 hit receiving rolls
- If success, standard hit receive chance penalty does not apply for one turn

**Fire Control**:
If destroyed:
- Lasers must now roll 2+ on a d6 to hit
- -2 to particle cannon rolls
- -2 to missile hit rolls

**Heat Management**:
If destroyed:
- Cannot store heat at all
- Must continuously radiate

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
- Drawback: PD can be overwhelmed. Each PD system can only destroy 2 missiles. If the squadron has only 2 ships and 1 PD system between them, if 4 enemy ships each launch a missile, the attacker performs a hit chance roll for missiles 3 and 4. If number of missiles fired at the formation > 2x the number of active PD systems, then perform standard hit chance rolls for every missile fired after the missiles that will be destroyed, in the same turn.

**2. Attack Line**
- Requirement: Ships in linear formation 6" apart
- Benefit: Combined targeting data (+1 per ship in line to all hit rolls)
- Drawback: Enemies receive +1 to all hit rolls when flanking (any attack from >45° off the line's axis) the line

**3. Screening**
- Requirement: Two ships forward of ship or ships being screened, max 9" apart
- Benefit: Forward ships can mask heat signatures of rear ships (i.e. rear ships can radiate without being detected thermally) and share targeting data with rear ships
- Drawback: Forward ships can be shot at by enemies from beyond even long range of the rear ships

**4. Dispersed**
- Requirement: No ships within 9" of each other
- Benefit: If two ships attack a single target from opposing directions, both ships get a +2 to hit rolls
- Drawback: No mutual support

### Victory Conditions
- Destroy all enemy ships
- [Further development possible here]

