### Components Needed To Play
- D6 dice (at least 2 per player)
- D10 dice (at least 1 per player)
- Ship miniatures (Anything roughly ship-shaped and about 2 inches in length including sausages, if you send a photograph of a particularly funny miniature stand-in, I will put it the repository)
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
- Engine (Destruction = Ship Lost) (This has one point of armour as the most important system)
- Magnetic Field (Damage = 9G limit)
- Fire Control (Damage = Hit penalties)
- Heat Management (Damage = No heat storage)
- Missile Bays (Damage = Lose missiles)
- Point Defense (Damage = Missile vulnerable)

### Turn Sequence
Each game turn consists of five phases, executed in order:

#### 1. Heat Management Phase

Player each roll a D10 to determine which player is high initiative for the duration of the turn.

**Heat Management System**
- Add heat from previous turn's actions
- Each ship must choose and declare:
  - Store heat (remain stealthy, invisible to thermals, standard hit receiving chance)
  - Radiate heat (visible to thermals, if also visible to visual, attack rolls get a +1 bonus against you) - radiates 10 heat per turn

**Critical Heat Threshold**: 30
- Going over causes one internal damage point to the heat management system
- 3 internal damage points
- Remain in this state for 3 turns and your heat management system explodes, exceeding 30 just causes and internal damage point  but allows continued heat accumulation

**Destroyed Heat Management System Effects**:
- Must continuously radiate
- Maximum storage with destroyed system is 20
- If a ship exceeds 20 heat with a destroyed heat management system at the damage resolution phase (phase 5), that ship is destroyed 

#### 2. Movement Phase
- Player with high initiative moves one ship first, then the player with low initiative moves
- Repeat until all ships have moved

**Movement Capabilities**:
- Frigates: Up to 29G with functioning magnetic system (other classes to be added in the future)
- 2D Movement - 3D is a bit hard on a tabletop
- In order to avoid players having to calculate vector dot products, movement has been heavily abstracted
- These frigates are small, fast ships with fighter levels of mobility
- From stationary, you can burn in any direction up to 29G
- Each G represents 1" of movement
- To represent that the ship is already in motion, a burn in the same direction as previous motion up to 45 degrees off the line of previous motion has a -2 to the heat cost of the movement (this is not how adding an acceleration vector to an existing velocity vector works but it is abstracted for gameplay purposes)
- Applying the same logic, a burn in a direction between 46 - 90 degrees off the line of previous motion has a -1 to the heat cost of the movement.
- To turn more than 90 degrees (i.e. in the opposite direction), subtract distance moved in the preceding turn from the maximum movement ability, and that is that ship's maximum movement beyond 90 degrees for that turn, and also represents a minimum heat cost. 
- For example, if a ship makes a 29G burn in the previous turn, it cannot move in a direction more than 90 degrees off its current path, and to stay in place will cost a 29G burn
- Players are not allowed to not burn at all due to the abstraction to prevent players having to do vector mathematics
- You can point in any direction after moving, but this is irrelevant since formation bonuses depend on direction of motion and the guns are on turrets

**Heat Generation Table**:

| G-Force | Heat Generated |
|---------|----------------|
| 1-4G 	  | 1 heat   	     |
| 5-9G 	  | 2 heat   	     |
| 10-18G  | 3 heat   	     |
| 19-24G  | 4 heat   	     |
| 25-29G  | 5 heat   	     |

**G-Force Hit Receiving Modifications**:

| G-Force | Roll Difficulty Modification |
|---------|------------------------------|
| 1-4G 	  | - 2         	                |
| 5-9G 	  | - 1         	                |
| 10-18G  | + 0         	                |
| 19-24G  | + 1         	                |
| 25-29G  | + 2         	                |

**G-Force Movement Rules**:
- Base movement: 1" per G

**Movement Restrictions**:
- Must declare G-force before moving
- Cannot exceed maximum G based on system status
- All movement must be in straight lines

#### 3. Detection Phase

Check each ship's visibility:
- Radiating heat = Automatically detected
- Visual range ~30 miles (30" on table)
- Heat signatures reveal position
- Detected ships can be targeted but only by the ship that can detect it
- Targeting information cannot be shared unless using the screening tactic
- Ships radiating and in visual range give attackers +1 roll bonus to hit

#### 4. Combat Phase

1. High initiative player selects ship to fire
2. Low initiative player selects ship to fire
3. Continue alternating until all ships have fired or passed
4. Do not resolve damage until the next phase - this means that if a ship is killed or takes damage in this phase, the change in status will only take effect in the damage resolution phase.

Each ship can use one weapon system per turn:

**Laser System**:
- Costs 4 heat
- Always guaranteed hit
- Roll d6 for hit location for first shot
- Mark component on ship card as currently being burned by a laser
- Subsequent laser shots from the same attacking ship or another attacking ship require a 3+ roll from a 1d10 and it will do one point of damage that same component, if this second roll fails, remove the mark on card indicating it is being burned, and the attacker will roll a d6 again to determine where the laser hit, and mark that component as being burned
- Requires 2 consecutive hits on same location to kill a component
- Defender can choose to evade:
  - Declare before hit location roll but AFTER attacker declares laser firing
  - Loses their next shooting action
  - Negates the hit entirely
  - Evasion is a 1-9G burn in any direction, with the attendant low-G movement penalties and movement heat buildup (unlike regular movement, this is to be treated as a move from stationary)

**Particle Cannon**:
- Costs 8 heat
- Range requirements:
  - Long Range: roll at least 9+ using 2d20, then roll d6 for hit location
  - Mid Range: roll at least 6+ using 2d20, then roll d6 for hit location
  - Close Range: Guaranteed hit, roll d6 for hit location
- Hit does one point of damage to that that component
- No defence possible

**Missile System**:
- Each ship starts with 4 missiles
- Can only target ships with destroyed PD
- 66.6% chance to hit (roll 3+ on d6)
- Max range of 30" because your missile needs to constantly burn reaction mass to manoeuvre in space
- Scores a point of damage on hit (roll d6 for component)
- Unable to use if missile bays destroyed
- Can fire 2 missiles at once, but remember, ships with active PD are completely invulnerable to missiles

#### 5. System Status Phase

- Check component damage on all ships
- Resolve system effects
- Update ship status cards

### Damage Resolution

#### Component Damage Effects

#### Hit Location Table
| D6 Roll | Component Hit   | Damage points required for destruction |
|---------|-----------------|----------------------------------------|
| 1       | Engine          | 2                                      |
| 2       | Magnetic Field  | 1                                      |
| 3       | Fire Control    | 1                                      |
| 4       | Heat Management | 1                                      |
| 5       | Missile Bays    | 1                                      |
| 6       | Point Defense   | 1                                      |

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
| 10-15G  | 7+ on d10     |
| 16-20G  | 8+ on d10     |
| 21-24G  | 9+ on d10     |
| 25-27G  | 10 on d10     |

*GLOC Effects*:
- No actions for turn (no movement, cannot react)
- -3 hit difficulty
- If success, standard hit receive chance penalty does not apply for one turn
- For burns > 15G, if the player fails the GLOC roll, the player must roll at least 4+ on 1d6. If the player fails this roll, the crew of that ship dies.

**Fire Control**:
If destroyed:
- Lasers must now roll 2+ on a d6 to hit
- +1 to particle cannon roll difficulty
- +1 to missile hit roll difficulty

**Heat Management**:
If destroyed:
- Cannot store heat at all
- Must continuously radiate

If heat > 30:
- Add one internal damage point to that ship's heat management system

**Missile Bays**:
If destroyed:
- Lose all remaining missiles
- Cannot launch missiles

**Point Defense**:
If destroyed:
- Ship becomes vulnerable to missiles
- No defense against incoming missiles

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
- Drawback: Does not provide any offensive bonuses

**2. Attack Line**
- Requirement: Ships in linear formation 6" apart. In the preceding movement phase, all ships' movement must be within 30 degrees of parallel motion
- Benefit: Combined targeting data (-1 to roll difficulty per additional ship in line other than firing ship to particle cannon hit rolls)
- Drawback: Enemies receive -1 to particle cannon hit roll difficulty when flanking (any attack from >45° off the line's axis) the line

**3. Screening**
- Requirement: Two ships forward of ship or ships being screened, max 9" apart. In the preceding movement phase, all ships' movement must be within 30 degrees of parallel motion
- Benefit: Forward ships can mask heat signatures of rear ships (i.e. rear ships can radiate without being detected thermally) and share targeting data with rear ships, rear ships firing on same ship as a screening ship receives a 1- to particle cannon hit roll difficulty.
- Drawback: Forward ships are particularly vulnerable to offensive focused formations

**4. Dispersed**
- Requirement: No ships within 9" of each other
- Benefit: If two ships attack a single target from opposing directions (if you draw an imaginary line between the target ship, both attacking ships must be within 30 degrees of the line, and both must attack the target ship in that turn), both ships get a -1 to particle cannon hit roll difficulty
- Drawback: No mutual support

### Captains

#### Setup

At the start of the game, before starting play, players have 4 captains with unique bonuses to assign to their ships. Each ship can only have one captain.

The player must mark (privately) which ship has each captain on cards, and place those cards face down. Here are the captains:

**The Physicist**

This captain has three PhDs but can't remember where they put their coffee mug five minutes ago. Was recruited to the navy after accidentally creating a miniature black hole during a university experiment that somehow improved particle weapon efficiency. 
Spends off-duty hours scribbling incomprehensible equations on any available surface, including sleeping crewmates (not the only one who does this in the navy and it's only ever punished if the equations are wrong because those people shouldn't be allowed 
near particle weapons). Once per battle, can activate  what the crew nervously calls "the button we don't talk about" - a jury-rigged modification to the particle cannon that makes physicists at fleet command wake up in a cold sweat without knowing why. 
Limited to once per battle because the focusing crystal shatters in the process, and the science team has hidden the replacements after "the incident"  that left a perfectly spherical hole in the mess hall.

**Effect**: For one turn, the particle cannon shot is capable of punching through one unit of armour and destroying the component beneath it, instead of having to destroy the armour and the component with two separate shots

**The Tactician**
This captain's quarters are wallpapered with battle diagrams, and they've been caught moving salt and pepper shakers into formation patterns during meals. Regularly corrects historical battle accounts in their personal time and has been banned from three 
different military  history forums. Has memorised what every terminal does in the combat information centre. Once per battle, can enter what the crew calls "the zone" - a state of tactical clarity so intense that regular orders stop and what is being emitted 
vocally is just a stream of instructions to everyone across the entire formation on what to do at their battle stations. Nobody really understands what exaclty is happening but they just do it because they've seen it work before. Limited to once per battle 
because afterward the captain spends hours  explaining why it worked to anyone unfortunate enough to be trapped in  conversation.

**Effect**: For one turn, every ship in the squadron in a formation receives a +1 bonus to all hit rolls, for lasers, if already being shot by a laser, you only need to roll 6+ on 1d10 instead of 7+, particle cannons get a +1 to roll, 
and missiles get a +1 to hit chance, but PD immunity still applies

**The Engineer**
This captain once fixed a critical reactor breach with duct tape and a protein bar wrapper. Sleeps in the engine room more often than their quarters and has been caught whispering sweet nothings to the heat exchangers. Once per battle, can perform what the 
crew calls "percussive  maintenance" on the heat management system - a series of precisely calculated kicks and punches to various panels that somehow dumps 20  units of heat instantly. Limited to once per battle because afterward, the chief engineer threatens 
to space the captain without a suit. While the chief engineer knows that the captain is essentially disabling safety limits on heat pumps, nobody is entirely how the captain's hardware-based programming approach works.

**Effect**: For one turn, the ship can radiate 20 heat instead of the usual 10 per turn

**The Pilot**
This captain failed the academy's navigation course twice but somehow graduated top of their class in practical flight exercises. Claims to have learned to fly by "feeling the ship's aura" and regularly ignores the navigation computer's increasingly 
panicked warnings. Can somehow tell when a ship's engines are further along the maintenance cycle than the numbers suggest because "it should be going faster". Once per battle, can execute "the impossible turn" - a maneuver so physics-defying that enemy gunners 
question their own sanity and miss  completely. Limited to once per battle because the ship's AI threatens to lock the captain out of the flight controls "for everyone's safety."

**Effect**: For one turn, this ship can dodge absolutely any shot after a successful hit roll has been made against it

### Victory Conditions
- Destroy all enemy ships
- [Further development possible here]

### Tables for quick reference

**Heat Generation Table**:

| G-Force | Heat Generated |
|---------|----------------|
| 1-4G 	  | 1 heat   	     |
| 5-9G 	  | 2 heat   	     |
| 10-18G  | 3 heat   	     |
| 19-24G  | 4 heat   	     |
| 25-29G  | 5 heat   	     |

**G-Force Hit Receiving Modifications**:

| G-Force | Roll Difficulty Modification |
|---------|------------------------------|
| 1-4G 	  | - 2         	                |
| 5-9G 	  | - 1         	                |
| 10-18G  | + 0         	                |
| 19-24G  | + 1         	                |
| 25-29G  | + 2         	                |

**Hit Location Table**

| D6 Roll | Component Hit   | Damage points required for destruction |
|---------|-----------------|----------------------------------------|
| 1       | Engine          | 2                                      |
| 2       | Magnetic Field  | 1                                      |
| 3       | Fire Control    | 1                                      |
| 4       | Heat Management | 1                                      |
| 5       | Missile Bays    | 1                                      |
| 6       | Point Defense   | 1                                      |

**GLOC Table**:

| G-Force | Required Roll |
|---------|---------------|
| 10-15G  | 7+ on d10     |
| 16-20G  | 8+ on d10     |
| 21-24G  | 9+ on d10     |
| 25-27G  | 10 on d10     |

**Weapon base roll table**

| Weapon          | Base Roll                        | 
|-----------------|----------------------------------|
| Laser           | 3+ on d10 (subsequent shot)      |
| Particle Cannon | 9+ on d10 (Long range)           |
| Particle Cannon | 6+ on d10 (Medium range)         |
| Missile         | 3+ on d10 (Can fire two at once) |
