# Grimware — Cyber Grimoire

Public static-site edition of Cyber Grimoire.

## Publish with GitHub Pages
This repository contains an automatic deployment workflow in `.github/workflows/pages.yml`.

1. Open **Settings → Pages** in the repository.
2. Under **Build and deployment → Source**, choose **GitHub Actions** (not "Deploy from a branch").
3. Open **Actions → Publish Grimware**, and use **Run workflow** if a run did not trigger automatically.
4. When the deployment succeeds, the website will be **https://carlosg888.github.io/Grimware/**.

## Required media assets
The app references these files, which must exist in the repository for graphics and audio to work:
- `Cyber_Grimoire_Sigil.png`
- `audio/brotherhood_empire_anna.mp3`
- `audio/shadow_alchemy_anna.mp3`

Upload them from the `Grimware_Public_Ready.zip` package to the same relative paths. Do **not** upload the ZIP alone.

## Privacy
The original author's embedded private dream entry was excluded from the public HTML. Entries created by visitors use browser localStorage; they are neither encrypted nor password-protected, and anyone using the same browser profile may access them. Do not treat this application as a secure vault.

## Ownership and licensing
The source and audio are not licensed for third-party reuse unless the owner adds an explicit license. Ensure permissions to distribute embedded audio and artwork publicly.

## Audio playback and troubleshooting
The public audio section now checks whether each MP3 is hosted. If absent, it disables **Play recording** and offers **Listen to guided narration**, a shorter browser-generated voice alternative without Anna's original voice, backing music, or timed silence. Users must tap to start speech (mobile browsers restrict autoplay).

To enable the **original** full-length tracks for all visitors, commit both MP3 files to the following exact paths (create the `audio/` folder if needed):
- `audio/shadow_alchemy_anna.mp3`
- `audio/brotherhood_empire_anna.mp3`

GitHub browser uploads can upload a batch of files from the extracted ZIP, but don't upload the ZIP alone. Once committed, wait for the GitHub Pages deployment and refresh the webpage. Check that direct URLs under `https://carlosg888.github.io/Grimware/audio/` load.

## Servitor Chamber (interactive)

Open **Solo Work → ✦ Servitor Chamber**.

- Guided 7-stage creation wizard: identity, purpose, boundaries, sigil, activation, maintenance, review/dissolution.
- Reproducible sigil generator with constellation, radiant and angular styles; colors and variation controls; PNG export.
- Each servitor has an editable purpose, instructions, ritual wording, boundaries, status (draft, active, paused, complete), and timestamped working journal.
- Search and filter saved records, duplicate or delete them, or export an individual servitor to JSON.
- Prior simple Servitor Forge entries are migrated to the new format when opening the chamber.
- Records are stored in the existing browser `localStorage` dataset and included in **Archive → Backups & Settings → Export backup**.

**Privacy warning:** The public GitHub Pages source contains only the chamber's application code. Visitors' records stay in their own browsers; no account-based sync is provided. Local browser data is not encrypted and may disappear if site storage is cleared. Export backups regularly and avoid entering confidential information on shared devices.

**Symbolic practice:** Servitors are presented as a voluntary chaos-magick / reflection practice. The program records ritual intentions and prompts actions; it makes no claim to autonomous spiritual or business results.

The feature requires all three files to be hosted at the repository root:
- `index.html`
- `servitor-chamber.js`
- `servitor-chamber.css`

