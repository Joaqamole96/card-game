# Standards for Legalistic Game Rules Documents (standards.md)

## 1. Purpose
This document defines the style, structure, and conventions to be used when generating game rules in a **legalistic, formal, and unambiguous** format. All such documents shall adhere to these standards to ensure consistency, clarity, and machine‑assisted maintainability.

## 2. Document Structure

### 2.1. Preliminary Definitions
Every rules document shall begin with a section titled **"Preliminary Definitions"** or **"§1 – Definitions"**. This section shall:
- List all capitalized terms that have a special meaning within the document.
- Define each term in a self‑contained manner, using the form: "**Term** means …".
- Cross‑reference the article or section where the term is further explained if necessary.
- State that the definitions apply throughout the document unless the context requires otherwise.

### 2.2. Article and Section Hierarchy
Documents shall be organized into **Articles** (major divisions) and **Sections** (subdivisions).
- **Articles** are numbered consecutively (Article 1, Article 2, …) and have a title.
- **Sections** are numbered within each Article (e.g., Article 1, §1.1, §1.1.1).
- Subsections may be used where needed; the numbering shall reflect the hierarchy (e.g., §1.2.1(a)).
- Each Article and Section shall be preceded by a descriptive heading.

### 2.3. End Matter
If needed, the document may include:
- A **Glossary** repeating key definitions.
- An **Index** of referenced sections.
- A statement of **Interpretation** (e.g., "In the event of any ambiguity, the game system's internal resolution shall prevail.").

## 3. Language and Style

### 3.1. Modal Verbs
Use the following modal verbs precisely:

|--------------|-----------------------------------------------------------------------------------|
| Verb         | Meaning                                                                           |
|--------------|-----------------------------------------------------------------------------------|
| **shall**    | Indicates a mandatory requirement. Violation is not permitted.                    |
| **must**     | Equivalent to "shall". Use consistently; prefer "shall" for rules.                |
| **may**      | Indicates a permitted action or option.                                           |
| **should**   | Indicates a recommendation, not a requirement. Avoid in core rules.               |
| **can**      | Indicates capability or possibility. Use sparingly; prefer "may" for permission.  |
|--------------|-----------------------------------------------------------------------------------|

### 3.2. Tense and Voice
- Use the **present tense** for rules that are continuously in effect.
- Use the **future tense** ("will") only when describing a guaranteed consequence that has not yet occurred.
- Prefer **active voice** ("the Player plays a card") over passive, but passive may be used when the actor is irrelevant ("the card is discarded").

### 3.3. Precision and Unambiguity
- Avoid pronouns where the referent could be unclear. Repeat the noun when necessary.
- Use "including but not limited to" when listing examples that are not exhaustive.
- Use "only if", "if and only if", or "unless" to define conditions with exact scope.
- Use **numbered lists** for sequences, options, or conditions that must be followed in order.

### 3.4. Terminology Consistency
- A single concept must be referred to by the same term throughout the document.
- Do not use synonyms unless they are defined as equivalent.
- Capitalize defined terms consistently (e.g., "Player", "Turn", "Figurehead").

### 3.5. Conciseness
- All text shall be the shortest possible while remaining exhaustive, exact, and complete.
- Filler, preamble, and illustrative examples shall be omitted unless the rule cannot be understood without them.
- Examples permitted under §4.5 are subject to this constraint.

## 4. Formatting Conventions

### 4.1. Headings
- Use **ATX headings** (`#`, `##`, `###`) for markdown.
- Article headings: `## ARTICLE X – TITLE`
- Section headings: `### §X.Y – Subtitle`
- Subsection headings: `#### §X.Y.Z – Sub‑subtitle`

### 4.2. Cross‑References
- Reference other sections using the format: **(Article X, §Y.Z)**.
- If the reference is within the same Article, use **(§Y.Z)**.
- When referencing a defined term, capitalize it and consider adding a parenthetical reminder of its definition on first use in a section.

### 4.3. Lists
- For sequences of steps, use numbered lists.
- For sets of conditions or non‑ordered items, use bullet lists.
- For definitions within a section, use a bullet or table with the term in bold.

### 4.4. Tables
Use tables for:
- Domain summaries, resource categories, evolution probabilities, etc.
- Each table shall have a clear caption or be introduced by a sentence that explains its purpose.

### 4.5. Examples
Examples may be placed in a block quote or italicized paragraph, prefaced by "**Example**:". They are illustrative and do not override the rule text.

## 5. Handling of Mechanics

### 5.1. Conditions and Triggers
- State conditions clearly: "If X, then Y." or "When X occurs, …".
- Distinguish between **continuous effects** ("While a Figurehead is present, …") and **one‑time triggers** ("When a card is played, …").

### 5.2. Simultaneous Resolution
- When actions resolve simultaneously, state that explicitly.
- Use language such as: "All declared actions resolve **simultaneously** at the end of the tick."

### 5.3. Priority and Conflicts
- Define a deterministic method for resolving conflicts (e.g., "by age, then by identifier").
- Indicate when the system handles priority without Player intervention.

### 5.4. Numerical Values and Ranges
- Use "zero (0)", "one (1)", etc., for clarity.
- Define caps explicitly: "ranging from zero (0) to one hundred (100), inclusive."

### 5.5. Queues and Delayed Actions
- Describe the queue as a first‑in, first‑out structure unless otherwise specified.
- State what happens when a queued action becomes impossible.

## 6. Internal Consistency
- All cross‑references must be accurate.
- No two rules may contradict each other. If an exception exists, it must be clearly stated (e.g., "Notwithstanding §X.Y, …").
- The document should be self‑contained; external documents may be referenced only by title and version.

## 7. Markdown and Presentation
- Use `---` horizontal rules sparingly, only to separate major sections.
- Prefer plain markdown; avoid HTML unless necessary for complex tables.
- Code blocks (triple backticks) may be used to show game data structures or examples.
- Ensure the document renders clearly in both raw markdown and rendered form.

## 8. Application for LLMs
These standards shall be applied to all future game rules expansions, card definitions, and scenario documents to ensure a uniform legalistic style. When an LLM is instructed to produce a rules document in this legalistic style, it shall:
1. Begin with a Preliminary Definitions section listing all capitalized terms.
2. Organize the content into Articles and Sections following the hierarchy.
3. Use "shall" for mandatory rules, "may" for optional actions.
4. Maintain consistent terminology and cross‑reference existing sections.
5. Avoid ambiguous language, metaphors, or colloquialisms.
6. Use tables and lists where appropriate to enhance clarity.
7. End with a short interpretation clause if applicable.

## 9. Document Versioning

### 9.1. – Version String Format
Every document filename shall include a version string in the format `X.Y.#.A`, appended before the file extension (e.g., `core.1.0.0.1.md`). Each component is defined as follows:

| Component | Type    | Sync Scope                                                                 |
|-----------|---------|----------------------------------------------------------------------------|
| X         | Integer | Major version. Increment requires all documents in the entire project to be updated to the same X value. |
| Y         | Integer | Minor version. Increment requires all documents within the same directory or system to be updated to the same Y value. |
| #         | Integer | Sub‑system version. Equivalent to Y but for a further nested subsystem or subdirectory. May be repeated as additional levels of nesting require (e.g., `X.Y.#1.#2.A`). |
| A         | String  | Document version. Increment affects only the current document. Not dependent on any other document. May be an integer, a character, or an alphanumeric string. |

### 9.2. – Incrementing Rules
1. When X is incremented, all documents in the project shall be updated and their X component set to the new value before any further work proceeds.
2. When Y is incremented, all documents within the affected directory or system shall be updated to the new Y value.
3. A may be incremented freely and independently of all other components.

## 10. Audits and Pending Items

### 10.1 – Regular Audits
Every major subsystem shall be audited for integration with the full rules at least once before final publication. Audits shall follow the format established, identifying:
- Undefined terms;
- Conflicts with existing rules;
- Ambiguities in timing, targeting, or magnitude;
- Gaps in resource or action integration.

### 10.2 – Pending Items
When a decision cannot be finalized during an audit, the relevant section shall be marked with a **PENDING** comment.

## 11. Subdivision of Large Systems

### 11.1 – Principle
As the rules expand, individual documents may become unwieldy. To maintain clarity and ease of reference, any system that meets one or more of the following criteria shall be subdivided into separate documents:
- The system contains more than **ten (10)** distinct sub‑components (e.g., cards, buildings, events) that each require detailed descriptions.
- The system's description exceeds **five (5)** pages in standard formatting.
- The system is mechanically independent and can function as a standalone module.

### 11.2 – Subdivision Procedure
When a system is subdivided:
1. Create a **master document** named after the system (e.g., `tarot.md`). Master documents shall **not** be named `README.md` or any generic index filename. The master document shall contain:
   - A table of contents linking to the sub‑documents.
   - Definitions and rules common to all sub‑components.
   - Cross‑references to the sub‑documents.
2. Create **sub‑documents** for each logical grouping (e.g., `major_arcana.md`, `minor_arcana.md`, `court_cards.md`).
3. Each sub‑document shall:
   - Begin with a reference to the master document.
   - Follow the same legalistic style and numbering conventions as the main rules.
   - Use consistent cross‑references (e.g., "as defined in Tarot Master Document, §3").
4. The main rules document may reference the master document without reproducing its contents.

### 11.3 – Example
- `tarot.md` – Overview, suits, positions, rank mechanics, cost, deck construction.
- `major_arcana/` – Separate files for each Major Arcana or grouped by theme.
- `minor_arcana.md` – Number cards (Ace–10) by suit.
- `court_cards.md` – Page, Knight, Queen, King rules, Figurehead summoning, lineage.

## 12. Redundancy
To minimize the need to cross‑reference multiple documents during gameplay, critical definitions and fundamental rules **shall** be repeated in sub‑documents where they are directly used. However, the authoritative definition remains in the core document. Redundancy applies to:
- Definitions of basic terms (e.g., "Turn", "Tick", "Domain").
- Core resolution mechanics (e.g., "simultaneous resolution", "priority").
- Commonly invoked rules (e.g., "Crisis of Succession", "card cost").

---

**END OF STANDARDS**