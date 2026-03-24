# Tarot Master Document

This document is the master reference for all Tarot card mechanics. It defines common rules that apply to all cards. Detailed rules for individual cards are contained in sub‑documents.

---

## 1. Overview
Tarot cards are the primary means by which Players influence the game state. Each card is defined by:
- **Position**: Upright or Reversed
- **Rank**: Ace through King
- **Suit**: Swords, Wands, Cups, Pentacles
- **Major Arcana**: The card’s archetype (e.g., The Fool, The Magician)

---

## 2. Card Components

### 2.1 – Position
Every Tarot card has a Position: **Upright** or **Reversed**.
- **Upright**: The card performs its effects as intended.
- **Reversed**: The card reverses its properties as follows:
  - **Domain inversion**: The Suit’s core purpose is inverted (e.g., Swords → pacification; Pentacles → resource drain).
  - **Target inversion**: Beneficial effects become harmful and vice versa; friend/foe targeting is swapped.
  - **Magnitude**: Numerical values are still multiplied by Rank (see §3.2) unless otherwise specified.
  - Position does not affect Rank multipliers or Court summoning mechanics.

### 2.2 – Rank
1. Rank corresponds to the traditional tarot card ranks: Ace, 2, 3, 4, 5, 6, 7, 8, 9, 10, Page, Knight, Queen, King.
2. Rank multiplies the strength or effectiveness of the card’s effect by the Rank’s numeric value:
   - Ace = 1
   - 2 = 2, … 10 = 10
   - Page = 11, Knight = 12, Queen = 13, King = 14

#### 2.2.1 – Count Value
The Count of a card is equal to its Rank value as defined in §3.2.

### 2.3 – Suit
The Suit determines the core purpose of the card:

|-----------|--------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| Suit      | Upright Purpose                                                                            | Reversed Inversion                                                          |
|-----------|--------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| Swords    | Attacks, defenses, imposing justice.                                                       | Pacification, disarmament, vulnerability, weakening offensive capabilities. |
| Wands     | Spreading religion, miracles, curses, omens, passion, silencing sedition.                  | Decline, stagnation, failed expansions, religious backfire.                 |
| Cups      | Building relationships, calming unrest, boosting morale, fostering unity and leisure.      | Discord, unrest, demoralization, social fracture.                           |
| Pentacles | Accumulating resources, building structures, enabling trade, funding expenses and tragedy. | Scarcity, decay, trade disruption, resource drain.                          |
|-----------|--------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|

---

## 3. Court Cards and Figureheads
See the dedicated document `court_cards.md` for detailed rules on Court cards and Figurehead summoning.

---

## 4. Major Arcana
Each Major Arcana is documented in its own file under `major_arcana/`. The list includes:
- [The Fool](major_arcana/the_fool.md)
- (others to be added)

---

## 5. Minor Arcana (Ace–10)
Numbered cards (Ace through 10) are documented in `minor_arcana.md`.

---

## 6. Deck Construction

### 6.1 – Count Limit
1. The sum of Count values across all cards in a Player’s deck shall not exceed the campaign limit.
2. The default campaign limit is two hundred fifty (250).

### 6.2 – Major Arcana Copies
No limit is placed on the number of copies of a given Major Arcana in a deck, unless otherwise specified by scenario rules.

### 6.3 – Suits
Suits are not drafted. All four suits are available to be drawn during play, subject to the Suit Focus rules (see Core Rules, Article 13).

---

## 7. Card Cost
Playing a card requires expenditure of Card Energy equal to the card’s Count (see Core Rules, Article 12 for details).