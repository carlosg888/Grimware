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
