# Care Guide — Missing Infographic Prompts

`cat-emergency-sheet.html` has 6 cards. Only 2 have an illustrated infographic
(`images/care-guide/choke-guide.png`, `images/care-guide/cpr-guide.png`). The other
4 are plain text/lists:

| Card (h2) | Has image? | id in HTML |
|---|---|---|
| 24-Hour Emergency Vets (Singapore) | No — contact list, doesn't need one | — |
| Signs You Need a Vet Now | **No** | — |
| Choking — Heimlich Maneuver | Yes | `#choking` |
| CPR — Cardiopulmonary Resuscitation | Yes | `#cpr` |
| If You Suspect Poisoning | **No** | — |
| Dangerous Foods | **No** | — |
| Toxic Plants | **No** | — |

The 4 candidates below would benefit from a matching infographic. Prompts are written to
reproduce the house style seen in `choke-guide.png` / `cpr-guide.png`:

- Flat vector infographic illustration, warm cream/parchment background (`#F7F4EC`)
- Deep forest green (`#1F4534`) and clay red/maroon (`#8A3B2B`) as accent colors, brass gold
  (`#C9A648`) hairline dividers
- Serif italic display headline (like Fraunces) in dark maroon or forest green + clean sans-serif
  body text
- Circular numbered step badges (dark red or forest green circle, white number)
- Thin-line icon inside a soft circular outline next to each step
- One consistent orange tabby cat character reused throughout, simple flat style, warm skin-toned
  human hands where a hand is shown
- Portrait orientation, roughly 1080×1400px, designed to be screenshotted/cropped as a single PNG
- No photorealism — same flat editorial-illustration style throughout, not a photo collage

Generate each at **1080px wide, portrait**, save as PNG, and drop into
`images/care-guide/<name>.png`. Then in `cat-emergency-sheet.html`, replace the `<ul>` block in the
matching section with an `<img class="sheet-infographic" src="images/care-guide/<name>.png" alt="...">`,
following the same pattern as the choking/CPR sections (keep the alt text descriptive — it currently
carries the full text content for accessibility).

---

## 1. Signs You Need a Vet Now → `vet-now-guide.png`

```
Flat vector infographic poster, warm cream/parchment background (#F7F4EC), in the house
style of a veterinary first-aid infographic series (deep forest green #1F4534 and clay red
#8A3B2B accents, brass gold #C9A648 hairline dividers, serif italic dark-maroon headline,
clean sans-serif body text, thin-line icons inside soft circular outlines, one recurring
orange tabby cat illustrated in simple flat style).

Title at top, bold serif italic, dark maroon: "SIGNS YOU NEED A VET NOW"
Subtitle below in gray: "Cats hide illness well — these signs mean go now, not tomorrow."

Below the title, a vertical list of 8 warning-sign rows, each with a small thin-line icon in a
circle on the left and two lines of text on the right:
1. Lungs/breathing icon — "Difficulty breathing" — open-mouth breathing or panting, never normal in a cat
2. Litter-box icon — "Straining to urinate" — little or no output, or crying in the box
3. Stopwatch icon — "A long or repeat seizure" — over 2–3 minutes, or more than one in a day
4. Cat lying down icon — "Collapse or unresponsiveness" — can't stand or walk normally
5. Droplet icon — "Uncontrolled bleeding" — or pale, white, or blue-tinged gums
6. Abdomen/belly icon — "A hard, swollen, painful abdomen"
7. Warning triangle icon — "Known or suspected poisoning"
8. Bandage icon — "Any trauma" — hit by a car, a fall, an animal attack, even if the cat seems fine after

Bottom banner in a rounded clay-red box: a phone icon + "When in doubt, call a clinic and
describe what you're seeing — it's free and tells you whether to come in immediately."
Small illustrated orange tabby cat sitting calmly in the bottom corner.
Portrait orientation, 1080x1400px, flat 2D vector illustration, no photorealism, no text
outside what's specified.
```

## 2. If You Suspect Poisoning → `poison-guide.png`

```
Flat vector infographic poster, warm cream/parchment background (#F7F4EC), same house style
as a veterinary first-aid infographic series (deep forest green #1F4534 and clay red #8A3B2B
accents, brass gold #C9A648 hairline dividers, serif italic dark-maroon headline, clean
sans-serif body, thin-line icons in soft circles, one recurring orange tabby cat character).

Title, bold serif italic, dark maroon: "IF YOU SUSPECT POISONING"
Subtitle: "Don't wait for symptoms to confirm it — act on suspicion alone."

A prominent rounded callout box near the top in clay red with a warning icon:
"Do NOT induce vomiting unless a vet or poison control specifically tells you to."

Below, 4 numbered circular step badges (dark red circle, white number) in a vertical list,
each with a thin-line icon and short instruction:
1. Bag/packaging icon — "Bring the evidence" — packaging, plant, or a sample of what was eaten
2. Droplet/shower icon — "Rinse exposed skin" — about 15 minutes of running water if it touched fur or skin
3. Phone icon — "Call your regular vet first" — if reachable; otherwise go straight to a 24hr clinic
4. Car icon — "Go now" — don't wait to see if symptoms appear

Small illustrated section at the bottom: simple flat icons of common culprits in a row —
a lily flower, a small bottle of medication, a mouse/rodent bait box, a bottle of household
cleaner — each with a small "x" or warning mark, captioned "Common causes: toxic plants, human
medication, rodent bait, household chemicals."
Small orange tabby cat illustration in the corner, calm pose.
Portrait orientation, 1080x1400px, flat 2D vector illustration, no photorealism.
```

## 3. Dangerous Foods → `dangerous-foods-guide.png`

```
Flat vector infographic poster, warm cream/parchment background (#F7F4EC), same house style
as a veterinary first-aid infographic series (deep forest green #1F4534 and clay red #8A3B2B
accents, brass gold #C9A648 hairline dividers, serif italic dark-maroon headline, clean
sans-serif body text, one recurring orange tabby cat character in simple flat illustration
style).

Title, bold serif italic, dark maroon: "DANGEROUS FOODS"
Subtitle: "Common kitchen items that are safe for people but not for cats."

A grid of 6 food icon cards (2 columns x 3 rows), each card a small rounded rectangle with a
flat-illustration icon of the food item, a red circle-slash "no" mark overlaid in the corner,
and a short caption below:
1. Onion + garlic bulbs illustration — "Onion & Garlic" — cooked, raw, or powdered
2. A dark chocolate bar square — "Chocolate" — especially dark chocolate
3. A bunch of grapes / raisins — "Grapes & Raisins"
4. A stick of sugar-free gum — "Xylitol" — in sugar-free gum & baked goods
5. A lump of raw bread dough — "Raw Bread Dough"
6. A glass of milk / dairy — "Milk & Dairy" — most adult cats are lactose intolerant

Small orange tabby cat illustration sniffing curiously near an empty food bowl at the bottom,
with a small caption: "When in doubt, keep it out of reach."
Portrait orientation, 1080x1400px, flat 2D vector illustration, no photorealism, no
additional text.
```

## 4. Toxic Plants → `toxic-plants-guide.png`

```
Flat vector infographic poster, warm cream/parchment background (#F7F4EC), same house style
as a veterinary first-aid infographic series (deep forest green #1F4534 and clay red #8A3B2B
accents, brass gold #C9A648 hairline dividers, serif italic dark-maroon headline, clean
sans-serif body text, one recurring orange tabby cat character in simple flat illustration
style).

Title, bold serif italic, dark maroon: "TOXIC PLANTS"
Subtitle: "Common houseplants that are genuinely dangerous for cats."

Top: one large featured illustration card for the highest-risk plant, visually bigger than
the rest — a flat illustration of a lily flower with pollen visible, red "most dangerous"
ribbon/badge, caption: "Lilies — even pollen groomed off fur can cause kidney failure."

Below it, a second featured card, same size treatment: a flat illustration of a sago palm,
caption: "Sago Palm — every part is toxic, can cause liver failure."

Below that, a row/grid of 6 smaller plant icon cards, each a simple flat botanical illustration
with a small red "x" mark and one-word caption:
Aloe Vera, Poinsettia, Dracaena, Cyclamen, Asparagus Fern, Jade Plant, Snake Plant
(arrange as a neat 3-column grid, wrapping to 2 rows)

Small orange tabby cat illustration curled up safely away from a shelf of plants at the
bottom.
Portrait orientation, 1080x1400px, flat 2D vector illustration, no photorealism, no
additional text.
```

---

### After generating

1. Save PNGs to `images/care-guide/vet-now-guide.png`, `poison-guide.png`,
   `dangerous-foods-guide.png`, `toxic-plants-guide.png`.
2. In `cat-emergency-sheet.html`, swap each section's `<ul>...</ul>` for an `<img class="sheet-infographic" src="images/care-guide/<file>.png" alt="...">`, mirroring how `#choking` and `#cpr` are structured (lines 294–301).
3. Keep the underlying text somewhere accessible (either in the `alt`, same as choking/CPR, or leave a `<details>` with the plain list as a fallback) so the content isn't only conveyed by pixels.
