# SKFanartShotSource

A working archive of **model sheets**, **story plates**, and **prompt modules** for Soul Knight fan cinema: comics, short videos, animations, and key art.

Everything here is versioned, reviewable, and easy to pull. Large prompt libraries and reference images do not belong in a zip file or behind an upload limit on Discord, so they live here instead, where a costume revision is a commit you can read.

Open [`main.html`](main.html) in a browser for the illustrated tour.

---

## Why this exists

Generated characters drift. Hair loses a hand of length between panels, a sash forgets its trim, someone gains two inches the moment the camera moves.

This archive stops the drift before it reaches the render. Every character has one sheet, and that sheet is the only thing a prompt is allowed to describe from. The prompts do not paraphrase a design. They point at it and refuse substitutions.

Three rules travel with the files:

1. **Sheet authority.** The model sheets are the sole reference for every visual attribute. Nothing reaches a render unless it appears on the sheet first, and no detail is invented, altered, or quietly dropped.
2. **Locked continuity.** Retrieval anchors hold appearance, environment, lighting direction, and eye level steady from one panel to the next. Weapons stay static props unless a shot calls for them.
3. **Read in the open.** Revisions arrive as commits and pull requests, so the canon carries a history rather than a folder of files named final and final two.

---

## What is inside

| Kind                          | Count |
| :---------------------------- | ----: |
| Character model sheets        |    34 |
| Scene plates and story frames |    14 |
| Prompt modules                |    22 |
| Video takes                   |     4 |
| Total files                   |    74 |

Three casts are covered: the **Knight Gang**, the **Tao Gang**, and the **Pantheon of Three**.

---

## Repository structure

### `KnightGangRefs/` · 20 sheets

Full turnarounds for the Knight Gang, from the founding four through the Werewolf, the Robot, and the Interdimensional Traveler. Each sheet carries the front, both profiles, the back, and portrait insets, so a prompt can be held to any angle.

### `TaoGang_ModelSheets/` · 10 sheets

The monastery cast, including an unarmed pass on the Sword Master and a second reading of the Yin Yang Adept. Use these for pose, outfit, and proportion continuity.

### `the_pantheon_of_three/` · 10 files

Sheets, a prompt library, and two scene renders for the trio. Split three ways:

- `the_pantheon_of_three_model_sheets/` for Costume Prince, Warliege, and Trickster
- `the_pantheon_of_three_prompt_library/` for the per character reference prompts and the spotlight walk staging file
- `the_pantheon_of_three_scene_renders/` for the final key art and the same hall kept as a cleared plate

### `tao_gang_meetup_comic_assets/` · 6 files

Three finished comic plates and the continuity prompts behind them, split by the beat each one covers. Good for multi panel work where recognition has to survive across the whole sequence.

### `scene_introduce_rogue_to_tao_gang/` · 22 files

The largest folder, and the closest thing here to a full production. A tea room conversation cut as three continuous segments:

- `scene_opening_frames/`, `scene_transition_frames/`, `scene_closing_frames/` for the plates that hand one shot to the next
- `scene_prompt_modules/` for the three segments, written in several dialects so you can pick the one your tool likes
- `scene_video_materials/` for four takes that were held back from the cut
- `scene_dialogue_text/` for the script
- `Setting_Extraction_and_Replication/` for the schema that reads an environment out of a plate and rebuilds it without the characters

### `knight-gang-selfie-assets/` · 2 files

The founding four group shot and the request that built it, down to who holds the camera and where the device has to be.

### `no_discord_no_concord_assets/` · 2 files

A setting plate and an eight second video prompt for the confrontation among the ruins, written shot by shot with timings.

### `selfie_prompt_modules/` · 2 files

The reusable selfie request in both XML and JSON, carrying the sheet authority block that the rest of the library leans on.

### `.gitignore`

Keeps platform clutter such as `.DS_Store` out of version control.

> Folders evolve. Check the commit history for the current intent behind any of them.

---

## Getting started

### Clone the repository

```bash
git clone https://github.com/Funny-Youngster/SKFanartShotSource.git
cd SKFanartShotSource
```

### Browse the archive

```bash
open main.html          # macOS
xdg-open main.html      # Linux
start main.html         # Windows
```

The page reads the images and videos straight from the folders, so there is no build step and nothing to install. Its one network request is the web font stylesheet from Google Fonts. Without a connection the page still works in full and falls back to system fonts.

### Render a shot

1. Pick the model sheets for everyone who appears in frame and attach them as reference images.
2. Pick a prompt module that matches what you want. Start from `selfie_prompt_modules/` for character portraits, `tao_gang_meetup_comic_assets/` for sequences, or `scene_introduce_rogue_to_tao_gang/scene_prompt_modules/` for video.
3. Keep the sheet authority block intact. It is the part that stops the drift.
4. Feed the previous plate back in as the environment anchor when you continue a sequence.

---

## Contributing

Fork it, extend a cast, add a scene pack. A few things keep the canon usable for everyone:

- Add a model sheet before you add prompts that depend on it.
- Keep one character per sheet, drawn as a full turnaround.
- When you revise a design, commit the sheet and say what changed in the message. That message is the changelog.
- Name new folders after the scene or cast they serve, not after the tool that made them.

---

## Credits

Kept by [@Funny-Youngster](https://github.com/Funny-Youngster) and [@LostInHustle](https://github.com/LostInHustle).

Soul Knight is a trademark of ChillyRoom. This is an unofficial archive built by fans and carries no affiliation with the studio.
