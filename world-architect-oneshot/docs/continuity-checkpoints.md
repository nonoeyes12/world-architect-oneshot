# Continuity Checkpoints — Keeping the World Connected

The most common failure of AI-generated settings is *orphaned lore*: beautiful details that
connect to nothing and never touch play. This framework fights that with checkpoints run **as
gates during generation**, a set of global invariants, and a required proof-of-connectedness
deliverable.

## The Principle

Every element must connect **backward** to a cause (history, resource, belief, or power) and
**forward** to play (a clue, choice, encounter, faction move, or ending). If an element connects to
nothing, it is cut or connected before the build continues.

## The Gates

| After building… | The checkpoint |
|---|---|
| World Bible | Every institution, law, and custom traces to a stated history/resource/belief; the central contradiction is planted. |
| The Hidden Truth | It is foreshadowed by ≥3 concrete details already established. |
| Central Tension | Each force is embodied by a real faction, NPC, and location — no faceless abstractions. |
| Factions | Each links to ≥2 others and to the hidden truth. |
| Locations | Each holds ≥1 clue/NPC/faction presence and links to ≥2 others via routes. |
| NPCs | Each ties to ≥2 others, joins/opposes ≥1 faction, and guards ≥1 clue or secret. |
| Secrets & Clues | Every clue sits in a named location/NPC; every secret is reachable by ≥2 independent paths. |
| Encounters | Each uses an established location and NPC/faction and moves the clock, a relationship, a resource, or a clue. |
| Escalation Clock | Every stage moves an element that already exists — no new orphans at escalation. |
| Finale & Endings | Each ending answers a prior choice, pays off the central contradiction, and resolves ≥1 planted secret. |

## Global Invariants

- No proper noun appears only once.
- Every clue points to something real; every secret is discoverable.
- Every faction can act in the finale.
- The chain **history → institutions → factions → conflicts → secrets → clues → choices → endings**
  is unbroken end to end.

## The Deliverable: A World Continuity Map

Before the run sheet, the model emits a table naming, for every faction, key NPC, key location, and
major secret: the **cause** it springs from, the **other elements** it connects to, the **clue(s)**
it holds or points to, and the **ending(s)** it can shape. If any row connects to nothing, the
campaign is revised until it does. (See the map at the end of the sample campaign in
[`../examples/`](../examples/) for a worked example.)
