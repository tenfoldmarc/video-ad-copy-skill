# Video Ad Copy
### A Claude Code Skill by [@tenfoldmarc](https://www.instagram.com/tenfoldmarc)

Tell Claude what you're promoting and how you'll shoot it. It writes a ready-to-record video ad script: 5 to 10 hook options, every spoken line with a timestamp, the on-screen text, the b-roll cue, and 15, 30, and 60 second cuts. Or, if you're making the video with AI (Seedance 2.5, Kling, Veo, Arcads), it writes a shot-by-shot list with a paste-ready prompt for every shot.

It knows your business after one short interview, and that profile is shared with the `/ad-copy` and `/ad-image-gen` skills.

---

## What It Does

1. First run only: a short interview, one question at a time. Skip anything. Saved as a profile so you never explain your business again. If you already ran `/ad-copy`, it skips this.
2. Asks what today's video is for, the format (talking head, UGC, AI avatar, or AI shot list), and whether the traffic is cold, warm, or hot.
3. Picks two different frameworks (PAS, UGC story, founder to camera, mini VSL, and 7 more) so you test real angles.
4. Writes 5 to 10 hooks of different types and marks the top 3, each with its first-frame text.
5. Writes the full script with timestamps, on-screen text, and visual changes every 3 to 5 seconds.
6. Delivers 15, 30, and 60 second cuts, plus delivery notes for the camera or the AI avatar.
7. Checks retention rules and Meta ad policy, saves everything, and learns from your results.

---

## Commands

| Type this | What it does |
|---|---|
| `/video-ad-copy` | Write a video ad for your active profile |
| `/video-ad-copy setup` | Run or re-run the interview |
| `/video-ad-copy edit` | Change one answer |
| `/video-ad-copy new [name]` | Add a second offer or a client |
| `/video-ad-copy profiles` | Switch between profiles |
| `/video-ad-copy results` | Tell it which script won |

---

## Requirements

- A Mac, Linux, or Windows computer
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) installed and working

No API keys, no extra tools.

---

## Install

No terminal needed.

### Step 1: Open Claude

Open the Claude Desktop app (or Claude Code, if you already use it).

### Step 2: Paste this message

```
Install this skill for me: https://github.com/tenfoldmarc/video-ad-copy-skill
```

### Step 3: Run the skill

```
/video-ad-copy
```

<details>
<summary>Prefer the terminal? Manual install</summary>

```bash
git clone https://github.com/tenfoldmarc/video-ad-copy-skill ~/.claude/skills/video-ad-copy
```

Then type `claude` and run `/video-ad-copy`.
</details>

---

## Usage

**Talking head for a free training**
```
/video-ad-copy Free training on booking sales calls with cold email. I'm on camera. Cold traffic.
```

**AI avatar UGC script**
```
/video-ad-copy UGC style script for the $97 course, I'll make it in Arcads.
```

**Seedance shot list**
```
/video-ad-copy Shot list for Seedance 2.5, 30 seconds, promoting the back pain video.
```

**Feeding results back**
```
/video-ad-copy results Script 2 hook 3 had a 42% hook rate, $6 CPL.
```

---

## What's Inside

- `SKILL.md`: the skill
- `reference/video-ad-frameworks.md`: 11 hook types, 11 script frameworks, retention rules, on-screen text rules
- `reference/shot-list-format.md`: the shot table, per-shot prompt structure, notes for Seedance 2.5, Arcads, Kling, Veo, Sora

Your profile lives at `~/.claude/ad-profiles/` on your machine and is shared with [ad-copy](https://github.com/tenfoldmarc/ad-copy-skill) and [ad-image-gen](https://github.com/tenfoldmarc/ad-image-gen-skill).

---

## Updating

Paste this into Claude:

```
Update the video-ad-copy skill from https://github.com/tenfoldmarc/video-ad-copy-skill
```

---

## Built By

[@tenfoldmarc](https://www.instagram.com/tenfoldmarc). Follow for daily AI automation walkthroughs. Real systems, not theory.
