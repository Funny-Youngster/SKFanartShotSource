# SKFanartShotSource

A complete, open-source collection of **source images**, **model sheets**, and **creative prompt modules** designed for generating **Soul Knight–themed** videos, comics, animations, and other visual content.

This repository exists so that large, evolving prompt libraries and reference images don’t have to live in oversized zip archives or get blocked by upload limits on platforms like Discord. Instead, everything is versioned, reviewable, and easy to pull, fork, and extend.

---

## Features

- **Centralized source of truth**  
  **Model sheets**, **reference packs**, and **prompt modules** for Soul Knight fanart workflows, all in one place.

- **Prompt-engineering ready**  
  Assets and prompts are organized around **scenes**, **characters**, and **shot types**, making them easy to plug into your own pipelines.

- **Version-controlled visual canon**  
  Character details (like outfit tweaks or scarf designs) are refined over time via commits and pull requests, keeping visual continuity tight.

- **Collaboration-friendly**  
  Designed to be forked, extended, and improved—whether you’re refining a model sheet or adding a new scene prompt pack.

---

## Repository structure

At a glance, the repo is organized into several top-level folders:

- **`KnightGangRefs/`**  
  Core reference images and/or sheets for the Knight Gang cast.  
  Useful for:
  - Character consistency across panels and shots  
  - Quick visual lookup while writing or prompting

- **`TaoGang_ModelSheets/`**  
  Model sheets for Tao Gang characters.  
  Useful for:
  - Pose, outfit, and proportion consistency  
  - Serving as a canonical reference for prompt engineering

- **`no_discord_no_concord_assets/`**  
  A consolidated asset pack originally created to escape Discord upload limits.  
  Think of this as a “misc but curated” bucket of useful resources.

- **`scene_introduce_rogue_to_tao_gang/`**  
  Assets and/or prompt modules for a specific narrative scene:  
  *introducing Rogue to the Tao Gang*.  
  Useful for:
  - Storyboard-style generation  
  - Reproducible cinematic setups

- **`selfie_prompt_modules/`**  
  Modular prompt snippets focused on **selfie-style** shots.  
  Useful for:
  - Character-focused close-ups  
  - Reusable prompt blocks for different characters or moods

- **`tao_gang_meetup_comic_assets/`**  
  Assets and prompts for a **Tao Gang meetup** comic sequence.  
  Useful for:
  - Multi-panel comic generation  
  - Maintaining continuity across a specific storyline

- **`.gitignore`**  
  Keeps platform-specific clutter (like `.DS_Store`) out of version control.

> Folder contents may evolve over time; check commit history and folder-level notes for the latest intent and usage patterns.

---

## Getting started

### Clone the repository

```bash
git clone https://github.com/Funny-Youngster/SKFanartShotSource.git
cd SKFanartShotSource
