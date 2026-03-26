VERSION: 1.0.0.2

# Leaders
This document defines the rules for leaders, including Figureheads, Tyrants, betrothment, lineage, and succession.

---

## PRELIMINARY DEFINITIONS
In these rules, unless the context otherwise requires:
- **"Leader"** means any Figurehead or Tyrant under a Player's control.
- **"Figurehead"** means a leader summoned by an Upright Court card.
- **"Tyrant"** means a leader summoned by a Reversed Court card, whose passive effect is the inverse of the corresponding Figurehead's effect.
- **"Role"** means the specific title held by a leader, as defined in §1.1.
- **"Betrothment"** means a declared bond between two leaders, as defined in Article 2.
- **"Heir"** means a non-leader entity produced by a betrothed Patriarch and Matriarch, as defined in §3.1.
- **"Crisis of Succession"** means the debuff applied when a Player's last Leader is removed, as defined in §1.2.

---

## ARTICLE 1 – LEADERS

### §1.1 – Roles
Each Court card summons a leader of a specific Role. The following table defines all Roles, their source card, and their Figurehead passive effect:

| Role      | Source Card | Figurehead Passive Effect                                   |
|-----------|-------------|-------------------------------------------------------------|
| Prince    | Page        | +1 Card Energy per Turn.                                    |
| Princess  | Page        | +1 Card Energy per Turn.                                    |
| Champion  | Knight      | +1 card drawn per Turn.                                     |
| Dame      | Knight      | +1 card drawn per Turn.                                     |
| Matriarch | Queen       | –1 cost for all Cards while alive.                          |
| Patriarch | King        | Significantly reduces the chance of drawing Reversed cards. |

For Reversed Court cards, the passive effect of the summoned Tyrant is the inverse of the Figurehead effect listed above. The exact inversion is determined by the game system.

#### §1.1.1 – Role Assignment on Summoning
1. When a Page Court card is played, the game system randomly assigns the summoned leader the Role of Prince or Princess with equal probability.
2. When a Knight Court card is played, the game system randomly assigns the summoned leader the Role of Champion or Dame with equal probability.
3. A Queen Court card always summons a Matriarch.
4. A King Court card always summons a Patriarch.

#### §1.1.2 – Role Uniqueness
Only one leader of any given Role may exist under a Player's control at a time. If a Court card is played and all Roles assignable by that card are already occupied, the card does not summon a leader and instead resolves as a Ten of the same Suit and Position (Court Cards Document, §3).

### §1.2 – Crisis of Succession
1. When the last Leader under a Player's control is removed, a Crisis of Succession occurs.
2. The Player receives a global card effectiveness debuff according to the following table, based on the Role of the removed Leader:

| Role      | Debuff Magnitude |
|-----------|------------------|
| Prince    | –1               |
| Princess  | –1               |
| Champion  | –2               |
| Dame      | –2               |
| Matriarch | –3               |
| Patriarch | –4               |

3. The debuff is applied once, only when the last Leader is removed, regardless of how many Leaders have previously been removed.
4. The debuff persists until any new Leader is summoned via any Court card, regardless of Position.
5. Summoning a new Leader immediately removes the debuff.

### §1.3 – Smiting
1. A Player may perform the "Smite" action (cost: one (1) Tick) targeting any Leader under the Player's control.
2. If the target is a Tyrant and the Culture Domain is eighty (80) or higher at the time of smiting, the population recognizes the tyranny and the Crisis of Succession debuff is **negated** (i.e., the debuff does not apply even though the last Leader is removed).
3. If the target is a Figurehead, §1.3.2 does not apply.
4. Future rebellion mechanics may build upon this negation.

### §1.4 – Leader Vulnerability
Events may kill Leaders. Any event text that indicates "may affect Leaders" does not specify odds; the outcome is determined by the game system.

---

## ARTICLE 2 – BETROTHMENT

### §2.1 – Declaration
1. A Player may perform the "Betroth" action (cost: one (1) Tick) to establish a betrothment between two eligible Leaders under the Player's control.
2. A Leader may be betrothed to at most one other Leader at any time.
3. A betrothed Leader may be re-betrothed only after the existing betrothment is dissolved (§2.2).

### §2.2 – Dissolution
A betrothment is dissolved when either betrothed Leader is removed from play by any means.

### §2.3 – Eligible Pairings
The following table defines which Roles may be betrothed to one another:

| Role      | May Be Betrothed To       |
|-----------|---------------------------|
| Patriarch | Matriarch, Dame           |
| Matriarch | Patriarch, Champion       |
| Champion  | Princess, Dame, Matriarch |
| Dame      | Prince, Champion, Patriarch |
| Prince    | Princess, Dame            |
| Princess  | Prince, Champion          |

---

## ARTICLE 3 – LINEAGE

### §3.1 – Heir Production
1. A Patriarch and a Matriarch who are betrothed to each other and have coexisted under the same Player's control for thirty (30) consecutive Turns produce an Heir at the end of that Turn.
2. The Heir's sex (Prince-line or Princess-line) is determined by the game system at the moment of creation.
3. An Heir is not a Leader and provides no passive bonuses.
4. Only one Heir may exist at a time. If a second Heir would be produced while an Heir exists, production is delayed until the existing Heir evolves or is removed.

### §3.2 – Heir Evolution
After ten (10) Turns as an Heir, the Heir evolves into a Prince (if Prince-line) or a Princess (if Princess-line), becoming a Figurehead with the corresponding passive effect (§1.1).

### §3.3 – Leader Evolution
At the end of each Turn, the game system checks for evolution according to the following probabilities (chances are approximate, determined by the system):

| From      | To        | Chance   |
|-----------|-----------|----------|
| Prince    | Champion  | High     |
| Prince    | Patriarch | Low      |
| Princess  | Dame      | High     |
| Princess  | Matriarch | Low      |
| Champion  | Patriarch | Very Low |
| Dame      | Matriarch | Very Low |

### §3.4 – Evolution Restrictions
1. Only one leader of a given Role may exist at a time.
2. If a leader would evolve into a Role already occupied, the evolution fails and the leader retains its current Role.
3. Matriarchs and Patriarchs cannot evolve further.

### §3.5 – Internal Priority
If multiple leaders would evolve into the same Role in the same Turn, the game system resolves the conflict internally (e.g., by age or identifier). The Player does not manage this process.

---

## ARTICLE 4 – INTERPRETATION
In the event of any ambiguity, the game system's internal resolution shall prevail. These rules are intended to be exhaustive; any effect not explicitly authorized is prohibited unless created by a card, event, or scenario rule.