# Pegger 3B Art Audit: What model Still Needs to Deliver

**Package:** `Pegger_Assets_3B.zip`, which contains every image currently in the game on branch `test-3b`. It uses the spec folder layout and filenames: `images/branding`, `backgrounds`, `guardians`, `guardians/avatars`, `gameplay`, `fx`, `ui`, `ui/badges` and `ui/concepts`.

**Contact sheets:** `contact_sheets/` shows every image on bright magenta. Any leftover painted background shows up as gray or black blotches.

| | Count |
|---|---|
| Images in the spec | 162 (161 original + the new `concept_fine_aim`) |
| Approved as delivered | 126 |
| **A. Missing** | 1 |
| **B. Regenerate: painted checkerboard or background** | 7 |
| **C. Regenerate: inconsistent or off-spec** | 14 |
| **D. Optional polish** (usable now) | 14 |

**Rule for this audit:** an image passes only when it meets every rule below. When model sends files back, check them off in the checklist at the end, or in `AUDIT_CHECKLIST.csv`.

---

## Delivery rules (paste these into model with the request)

1. **One image per screen,** with the screen named exactly the filename below, without the extension. No extra variants or duplicate takes. If you try several, send only the best one.
2. **Real transparency.** Export a PNG with an alpha channel.
   - **Never paint a gray or black checkerboard;** a painted checkerboard is not transparency.
   - If real transparency is impossible, use a perfectly flat **`#FF00FF` magenta** background, or **pure black `#000000`** for glass and glow objects.
   - No gradients, vignettes or texture in the background.
3. **No text or numbers** anywhere except the two logos.
4. **Centered,** with about 8% empty margin on every side. Nothing cropped, and no hard circular crop.
5. **Match the existing approved art:** same style, same top-left lighting, same character designs. When an item says "match X", put X next to it as a reference.

---

## A. Missing (1)

| File | Size | What to make |
|---|---|---|
| `ui/concepts/concept_fine_aim.png` | 256×256 | New concept icon for "Fine Aiming": a glossy dial knob with a tiny cannon and a short, precise dotted line, suggesting small careful adjustments. Chunky glossy 3D, matching the other concept icons (for example `concept_aim`). |

## B. Regenerate: painted checkerboard or background (7)

The art itself is approved. These only need a clean export with real transparency.

| File | Size | Problem | Fix |
|---|---|---|---|
| `branding/logo_pegger.png` | 2400×800 | A gray checkerboard is painted inside every glass letter bubble. It shows on the Home screen. | Same logo; the inside of each bubble must be clear glass with real transparency. |
| `guardians/guardian_pip_turtle.png` | 1024×1536 | A checkerboard is painted inside Pip's glass bubble helmet. | Same pose and design, clean transparent bubble. |
| `guardians/avatars/avatar_sage_turtledragon.png` | 512×512 | Checkerboard fragments around the whiskers on both sides. | Same portrait, clean background. |
| `guardians/avatars/avatar_mochi_panda.png` | 512×512 | A checkerboard shows through the green tea-steam swirl. | Same portrait, clean swirl. |
| `guardians/avatars/avatar_mochi_panda_worried.png` | 512×512 | A checkerboard fragment in the swirl at the right edge. | Same portrait, clean swirl. |
| `ui/dojo_aiming_lab.png` | 256×256 | A dark panel or shadow block sits behind the scope. | Icon alone on a transparent background. |
| `ui/concepts/concept_moving.png` | 256×256 | A dark streak panel sits behind the three orbs. | Three glossy orbs with soft motion streaks, transparent background. |

## C. Regenerate: inconsistent or off-spec (14)

| File | Size | Problem | Fix |
|---|---|---|---|
| `guardians/avatars/avatar_ember_phoenix.png` | 512×512 | Still the round-1 version, inside a gold medallion ring on a dark disc. Eight of the other Guardians are now unframed busts. | Unframed head-and-shoulders bust like `avatar_luna_fox`: orange-gold phoenix chick, flame crest, confident grin. |
| `guardians/avatars/avatar_ember_phoenix_worried.png` | 512×512 | Same framing problem. | Match the new `avatar_ember_phoenix` exactly; only the expression changes: flame crest drooping and flickering low, nervous grin, one blue sweat drop. |
| `guardians/avatars/avatar_pip_turtle.png` | 512×512 | Round-1 framed disc with a dark fragment on the right edge. | Unframed bust like `avatar_luna_fox`: mint-green young sea turtle, teal scarf, gentle smile. Match `guardian_pip_turtle`. |
| `guardians/avatars/avatar_pip_turtle_worried.png` | 512×512 | Round-1 framed disc. | Match the new `avatar_pip_turtle`: half-hiding behind the shell edge, worried eyes, one blue sweat drop. |
| `guardians/avatars/avatar_jinx_cat_worried.png` | 512×512 | **Off-model.** A flatter, different drawing with no purple vest, a different hat and a different face shape. | Match `avatar_jinx_cat` exactly (same vest, same striped top hat, same style); only the expression changes: ears flattened, crossed fingers held up, nervous smirk, one blue sweat drop. |
| `guardians/avatars/avatar_sage_turtledragon_worried.png` | 512×512 | Doesn't match the calm version: different horns, darker mustache, different robe and no tiara. | Match `avatar_sage_turtledragon` exactly; only the expression changes: whiskers twitching, brow furrowed, one blue sweat drop. |
| `guardians/avatars/avatar_bolt_squirrel.png` | 512×512 | A hard circular crop cuts off the tail and the left side; the other avatars are free-standing busts. | Same art as a free-standing bust with no circular crop and the tail fully inside the frame. |
| `guardians/avatars/avatar_bolt_squirrel_worried.png` | 512×512 | Lighter tan fur and a slightly different style from the calm Bolt. | Match the calm Bolt's chestnut fur, goggles and cape; only the expression changes: goggles askew, gritted-teeth nervous grin, one blue sweat drop. |
| `gameplay/peg_gold_lit.png` | 128×128 | Doesn't match the other lit pegs: no bright starburst core. | Same orb as `peg_gold`, lit in exactly the style of `peg_blue_lit`, `peg_orange_lit` and `peg_purple_lit` (white-hot starburst core, sparkling inner glow). |
| `gameplay/peg_green_lit.png` | 128×128 | Swirl-style glow instead of the shared starburst look. | Same as above, in green. |
| `gameplay/peg_flower_lit.png` | 128×128 | A large flower graphic instead of the shared starburst look, and the flower is far bigger than on the unlit `peg_flower`. | Same orb as `peg_flower`, lit in the shared starburst style, keeping the small flower motif. |
| `ui/mode_how_to_play.png` | 384×384 | Drawn inside a dark rounded-square app-icon tile; the other four mode tiles are free-standing objects. | Free-standing glowing storybook with a glass orb, transparent background, no tile behind it. |
| `ui/mode_quick_play.png` | 384×384 | Same problem: a dark rounded-square tile behind it. | Free-standing lightning bolt striking an orange glass orb, transparent background. |
| `ui/badges/badge_challenge_seeker.png` | 512×512 | **Contains text** ("GOAL 1 / GOAL 2 / GOAL 3"), which breaks the no-text rule and can't be translated. | Same medal with a checklist scroll that uses gold tick marks and plain lines, no words. |

## D. Optional polish (14 images)

The game works fine without these; they would improve quality.

| File | Delivered | Spec | Note |
|---|---|---|---|
| `backgrounds/bg_*.jpg` (all 10) | 848–896 px wide | 1536×2048 | Delivered at about half resolution and a slightly different aspect ratio. Sharp on iPhone, soft on iPad and Mac. Re-export at 1536×2048 with the same art. |
| `branding/splash_background.jpg` | 768×1376 | 1290×2796 | Not used in the game yet. Re-export at the spec size if model can. |
| `branding/app_icon_dark_1024.png` | opaque | transparent | iOS dark-mode icons look best with a transparent background behind the orbs. |
| `gameplay/ball_aqua.png` | 128×128 | | A faint horizontal seam across the middle. |
| `gameplay/fever_bucket_3.png` | 568×360 | | The 100K jackpot bin could be a bit more ornate than the other four: a gold crown flourish on the rim and a stronger golden glow. |

## Approved as delivered (126)

**Branding:** `logo_pegger_dark`, `title_fever`, `app_icon_1024`, `app_icon_tinted_1024`

**Guardians (full body):** Bolt, Ember, Jinx, Luna, Mochi, Nova, Rocco, Sage, Willow (all except Pip)

**Avatars:** `avatar_luna_fox` and its worried version, `avatar_nova_starfish` and its worried version, `avatar_rocco_crab` and its worried version, `avatar_willow_owl` and its worried version, and `avatar_jinx_cat`

**Gameplay:**
- 6 unlit pegs and 3 lit pegs (blue, orange, purple)
- 12 bricks and 6 of 7 balls (all except aqua)
- buckets, cannon, coins, bumper, portals, gravity well, dome, ice blocks, flipper, wheel, pointer and tutorial hand
- Fever bins 1, 2, 4 and 5 (bin 3 is in D only for optional polish)

**Effects:** all 9 particles

**UI:**
- 4 of 6 mode tiles (all except How to Play and Quick Play)
- Dojo cards for Bucket Catch, Fever Trainer and Power Playground
- `duel_vs` and all 8 icons
- 19 of 20 badges (all except Challenge Seeker)
- 12 of 13 concept icons (all except Moving)

---

## Acceptance checklist

When the new files arrive, each one must pass all of these before it counts as fixed:

- [ ] Filename matches exactly, in the right folder.
- [ ] Real transparency: on a magenta background there is no gray or black checkerboard, panel or vignette.
- [ ] Size matches the table, or at least the same aspect ratio at 1024 px or larger.
- [ ] No text, except the logos.
- [ ] Matches its reference: same character design, outfit, palette and lighting. Worried avatars differ from the calm ones in expression only.
- [ ] Centered with margin; nothing cropped.

| ✓ | File | Group |
|---|---|---|
| ☐ | `ui/concepts/concept_fine_aim.png` | A |
| ☐ | `branding/logo_pegger.png` | B |
| ☐ | `guardians/guardian_pip_turtle.png` | B |
| ☐ | `guardians/avatars/avatar_sage_turtledragon.png` | B |
| ☐ | `guardians/avatars/avatar_mochi_panda.png` | B |
| ☐ | `guardians/avatars/avatar_mochi_panda_worried.png` | B |
| ☐ | `ui/dojo_aiming_lab.png` | B |
| ☐ | `ui/concepts/concept_moving.png` | B |
| ☐ | `guardians/avatars/avatar_ember_phoenix.png` | C |
| ☐ | `guardians/avatars/avatar_ember_phoenix_worried.png` | C |
| ☐ | `guardians/avatars/avatar_pip_turtle.png` | C |
| ☐ | `guardians/avatars/avatar_pip_turtle_worried.png` | C |
| ☐ | `guardians/avatars/avatar_jinx_cat_worried.png` | C |
| ☐ | `guardians/avatars/avatar_sage_turtledragon_worried.png` | C |
| ☐ | `guardians/avatars/avatar_bolt_squirrel.png` | C |
| ☐ | `guardians/avatars/avatar_bolt_squirrel_worried.png` | C |
| ☐ | `gameplay/peg_gold_lit.png` | C |
| ☐ | `gameplay/peg_green_lit.png` | C |
| ☐ | `gameplay/peg_flower_lit.png` | C |
| ☐ | `ui/mode_how_to_play.png` | C |
| ☐ | `ui/mode_quick_play.png` | C |
| ☐ | `ui/badges/badge_challenge_seeker.png` | C |
| ☐ | `backgrounds/bg_*.jpg` (10) | D |
| ☐ | `branding/splash_background.jpg` | D |
| ☐ | `branding/app_icon_dark_1024.png` | D |
| ☐ | `gameplay/ball_aqua.png` | D |
| ☐ | `gameplay/fever_bucket_3.png` | D |

**Audio** is not part of this request. model can't produce it; see the ElevenLabs, Suno and Udio notes.
