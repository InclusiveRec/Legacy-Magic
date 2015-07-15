# Magic
MagicSpells configuration for server

ORGANISATIONAL TASKS:
- Standardise spell descriptions.  e.g.
    - (Colour code)Spellname: Lv(memory) (school) spell
    - Descriptive text
    - [Requires (prerequisites)]
- Standardise spell layouts:
    - spell-class
    - cast-item
    - spell-icon
    - casting costs (cost, cast-time, cooldown)
    - learning requirements (prerequisites, precludes, replaces, and memory)
    - spell-specific configuration (range, damage, etc)
    - modifiers
    - description and other strings
    - effects (particles, sound effects, etc)
- Most vital strings to write:
    - Descriptions
    - str-cost
    - str-modifier-failed (if spell has require/denied modifiers)

DESIGN TASKS:
- Technology tree
    - Item creation spells should require bind, unbind, and scroll spells (which I suppose can be implicit in prerequisite descriptions), as well as 1-2 beginner spells
    - Intermediate spells should require an item creation spell (pads out memory cost)
    - Every school needs a grimoire and appropriate item creation spells tied to it (a few exceptions are allowed, such as the magic sickle, which is too vital to forest/solar magic to be heavily restricted)
- Spell effects
    - Visual and sound effects are a great way to make spells characterful and "feel" magical.  If a spell doesn't have any built-in and obvious effects (like a fireball or particle projectile spell) it should have some effects.
    - Spell effects should give some hint as to the school they come from
    - Even simple spells like eating or item creation benefit from spell effects
    - You can accompany spell effects with str-cast-self, str-cast-target, or str-cast-others, but often these will not be necessary

