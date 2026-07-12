# The King's Reckoning — a math game on a living kingdom

![The King's Reckoning](share.jpg)

**A math game for 4th–7th graders, built on top of [*The Annals*](#the-annals-the-world-underneath) — a medieval realm that lives on its own.** The old Crown Reckoner is dead, and the kingdom needs a new one: **you.** Every coin in the treasury, every disaster averted, every village chartered is *paid for with arithmetic.* Math is the engine; the kingdom is the reward; and the realm's self-writing chronicle inks *your* deeds into history.

The kid isn't doing a worksheet with a screensaver behind it — the kid is holding the realm's purse, and the realm keeps living, prospering, and bleeding while they work.

**Play it: [annals-kingdom.netlify.app](https://annals-kingdom.netlify.app)**

Everything is one HTML file. No build step, no backend, no accounts. Your grade, rank, and mastery are remembered in your browser (localStorage); each new seed forges a fresh realm to reckon for.

## For kids, parents, and teachers

- **Target audience:** ages 9–13, U.S. grades 4 through 7 (adaptable to any child working at those levels).
- **A parent or teacher picks the grade band once** (a big Grade 4 / 5 / 6 / 7 card on the first screen). It is remembered and never changes on its own — only a grown-up moves it, via the 📜 Studies panel.
- **The game adapts *within* the grade.** A hidden 5-tier engine watches how you fare and quietly makes each skill gentler when you struggle and firmer (only when you're both correct *and* fluent) when you're ready. Struggling is always met with easier problems — never harder ones. There is **no game over and nothing is ever taken away**; a wrong answer costs only the streak and shows a kind clerk's note with the right answer.
- **What each grade band covers:**

  | Grade | Skills reckoned into the realm |
  |---|---|
  | **4** | multi-digit +/−, multiplication facts & 2×2, long division with remainders, place value, rounding, fraction basics |
  | **5** | decimal +/−/×/÷, fractions with unlike denominators, volume, order of operations, fraction-of-a-quantity |
  | **6** | ratios & rates, percentages, fraction × and ÷, negative numbers, one-step equations |
  | **7** | proportions, multi-step percent (discount + tax), integer operations, two-step equations, simple probability |

- **Progress data lives in the 📜 Studies panel:** a mastery bar per skill (Novice → Practised → Skilled → Master) — a quiet read-out of exactly which skills are strong and which need work.
- **Accessibility floor:** toggles for **Sound**, **Reduce Motion** (also honors your OS setting), and a **Gentle Realm** mode that stretches every timer by 1.5×. Correct/wrong never rely on color alone (a ✓/✕ glyph and the clerk's note always accompany it).

## How math drives the kingdom

The math panel has **three sections**, switched by tabs at the top of the Ledger: **✒ Ledger**, **🏰 Build**, and **⚔ Battle**.

- **✒ Ledger — gold is minted only by correct answers.** Each right answer pays real gold into the realm's actual treasury — the same number that governs whether villages get chartered and whether the dragon stirs. The free "grant gold" cheat of the base sim is switched off: the Reckoner's only faucet is arithmetic.
- **Streaks bloom the realm.** Consecutive correct answers grow a streak flame and its gold multiplier. At **5** a Festival lights the capital; at **7** and **10** a **Golden Age** actually buffs the kingdom's harvest, trade, and birth rates for weeks of sim-time. You make the realm prosper by stringing answers true.
- **🏰 Build — math raises a castle.** Spend earned gold to *commission* walls, watchtowers, a gatehouse, keep storeys, a moat, catapults, and a garrison — then every correct answer lays a stone until the piece rises on the castle diagram. Finished works add **defense** for the Battle section, and some carry perks: each keep storey pays +5% on every tally, the moat weakens attackers, catapults loose a free opening volley. Your castle is *yours* — it persists across realms and sessions. Battle damage shows up as scars you repair the same way: one true answer, one stone.
- **⚔ Battle — a war-board of turn-based math fights.** Choose a foe (Wolf Pack, Bandit Raiders, the Contagion, a Rival House Host, and — at high rank — the Dragon) and battle turns: a correct answer is a strike against the foe; a wrong answer or a timeout lets it hit your castle's defense. Win and you take plunder, glory in the chronicle, and (if you fought unerring) a chest. Lose and the foe merely withdraws with a little tribute — the realm is scarred but *never* lost. When something *real* stirs in the living sim — an actual bandit camp, a plague town, the waking dragon — that foe turns **urgent** on the war-board (a red dot marks the ⚔ tab), and beating it heals the real realm: the camp is scattered, the town cured, the dragon sent home.
- **Royal Decrees** are three small quests per session (count 12 tallies, hold a streak of 6, master a craft, win a battle unerring…), each with a chest at the end.
- **Ranks & Powers.** Lifetime correct tallies and mastered skills raise your Reckoner rank across seven titles (Apprentice Clerk → … → Grand Vizier). Higher ranks unlock **gold-priced Royal Powers** — bless the fields, charter a village, fund the watch, summon the rains, ward the dragon — so the gold you earn has somewhere to go.
- **Variable rewards.** Roughly one answer in eight drops a chest (bonus gold, a mastery surge, a "Golden Answer" token that triples your next reward, or a blessing); rare answers summon one of the world's own wonders as an omen.

Your best realm (its name and peak treasury) is remembered between sessions as a bragging-rights record, even though each seed is a fresh reign.

## Controls

The math **Ledger** is keyboard-first and touch-equal. Type your answer and press **Enter** (or tap **Reckon**); multiple-choice problems take keys **1–4** or a tap. Tabs at the top of the panel switch between **✒ Ledger**, **🏰 Build**, and **⚔ Battle**. The ✒ button (or `Q`) folds the Ledger away (never mid-battle); 📜 opens Studies & settings.

The living world underneath is driven exactly as *The Annals* always was:

| Desktop | Touch |
|---|---|
| drag to orbit | one finger orbits |
| wheel / trackpad scroll or pinch to zoom | pinch zooms |
| right-drag to pan | two fingers pan |
| double-click to travel | double-tap travels |
| click to inspect | tap inspects |

`space` pause · `1–5` speed · `T` territories · `C` watch mode · `G` director · `L` labels · `H` hide the court · `Q` fold the Ledger · `Esc` release

(While the answer box is focused, digit keys type into it rather than changing sim speed — so you can never fat-finger a pause mid-thought.)

## Running locally

Open `index.html` in a browser, or:

```
node server.js
```

and visit `http://localhost:8544`. The only network dependency is three.js r128 from a CDN.

## The Annals — the world underneath

The King's Reckoning is a layer on top of **The Annals**, a procedurally generated medieval realm that lives on its own and writes its own chronicle. All of it is still here, running while you reckon:

- **A forged world** — terrain, rivers that carve valleys and end in meres, biomes, pathfound roads, towns planned street by street, heraldry drawn house by house.
- **A working economy** — seven goods, prices from scarcity, caravans and cargo cogs you can follow down the roads, tolls, famines, and the occasional beached whale.
- **A dynasty** — named notables who marry, scheme, and die; successions, regencies, usurpers, browsable family trees; great houses with grudges and civil wars fought by armies that camp outside the walls.
- **The fates** — weather and floods, fires with real flames, plague waves, bandit kings, comets and eclipses, wolf-winters, white harts, and one dragon whose waking probability scales with the very treasury your math fills.
- **Towns that change** — houses rise with prosperity and rot with decline, forests are cleared into farmland, new villages are chartered over the decades.
- **An auto-director, Watch mode, the Chronicle, and Charts** — leave it alone and a camera drifts to whatever story is breaking; press `C` and the realm narrates itself; every event is inked with its date, filterable and exportable.

If you never open the math panel, the sim runs as a pure "watch the kingdom" experience, exactly as it always did.

### How it's built

Vanilla JavaScript and three.js r128, ~7,800 lines in one file. Four seeded RNG streams keep worldgen and simulation deterministic and independent — the same seed always yields the same world and history, at any speed. The math layer lives inside the same script, adds gold to the real treasury, buffs the real economy rates, and inks the real chronicle; its UI is pure DOM/CSS in the game's parchment style, and all its sound is synthesized in the Web Audio API with zero asset files, so the whole realm still draws in well under 100 draw calls at 60 fps.

## License

[MIT](LICENSE)
