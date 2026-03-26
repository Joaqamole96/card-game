VERSION: 1.0.1

# Core Rules
This document defines the fundamental structure of turns, time, and card play.

---

## PRELIMINARY DEFINITIONS
In these rules, unless the context otherwise requires:
- **“Player”** means any human or artificial intelligence participant in the game.
- **“Game State”** means the totality of all variables, including domains, population, resources, buildings, cards, and leader entities.
- **“Court Card”** means any Tarot card with Rank Page, Knight, Queen, or King.

---

## ARTICLE 1 – TIME AND TURN STRUCTURE

### §1.1 – Turn and Tick
1. **Turn**: A Turn represents a period of twenty‑four (24) hours within the game world.
2. **Tick**: Each Turn is divided into one thousand, four hundred and forty (1,440) Ticks. One Tick corresponds to one (1) minute.

### §1.2 – Turn Sequence
The conduct of each Turn shall follow the sequence set forth in this Section.

#### 1.2.1 – Start of Turn Phase
1. During the Start of Turn Phase, a Player may play any number of cards from their hand.
2. All cards played during this Phase are declared **simultaneously**, but resolve in an order determined by the game system (typically the order in which they were placed).
3. The cost to play a card (as defined in the Tarot Master Document, §4) is paid immediately upon declaration.
4. Playing a card consumes zero (0) Ticks.
5. After all card effects have resolved, the Turn proceeds to Tick Resolution.

#### 1.2.2 – Tick Resolution Phase
1. The Tick Resolution Phase consists of one thousand, four hundred and forty (1,440) consecutive Ticks, numbered 1 through 1,440.
2. **At the beginning of each Tick**, every Player shall declare all actions (as defined in the Actions document) that their forces will perform during that Tick.
3. All declared actions resolve **simultaneously** at the end of the Tick.
4. If an action cannot be completed because a target or required resource is unavailable at the moment of resolution, the action fails and produces no effect.
5. The game system shall automatically resolve internal priority conflicts (e.g., by age or identifier) without Player intervention.
6. After resolution, the Tick counter advances by one (1).

#### 1.2.3 – End of Turn Phase
1. After the one thousand, four hundred and fortieth Tick has resolved, the Turn ends.
2. Any actions placed in a pending queue (see Actions document, §6.2) are carried over to the next Turn and processed in order as resources become available.
3. The game system shall perform cleanup, check victory and loss conditions, and advance the Turn counter by one (1).

---

## ARTICLE 2 – CARD COST

### §2.1 – Energy Cost
Playing a card requires expenditure of Card Energy equal to the card’s Count (Tarot Master Document, §2.2.1).

### §2.2 – Modifications
The base cost may be modified by Figureheads, events, or other effects. The modified cost shall never be less than zero (0).

---

## ARTICLE 3 – SUIT FOCUS

### §3.1 – Declaration
At any point in the game, a Player may select any non‑empty subset of the four suits to be **active**.

### §3.2 – Drawing Restriction
Only cards whose Suit is active may be drawn from the deck.

### §3.3 – Changing Focus
The selection may be changed once per Turn, or as defined by the game’s action economy.

---

## ARTICLE 4 – INTERPRETATION
In the event of any ambiguity, the game system’s internal resolution shall prevail. These rules are intended to be exhaustive; any effect not explicitly authorized is prohibited unless created by a card, event, or scenario rule.

## ARTICLE (?) – START OF GAME
At the commencement of the game:
1. All Domains are set to fifty (50).
2. Population is set to the starting value specified by the scenario (default: one thousand (1000)).
3. Resources (Gold, Faith, Card Energy) are set to the starting values specified by the scenario.
4. No Figureheads or Heirs exist.
5. No buildings exist.
6. The Player possesses a starting deck of cards as defined by the scenario.