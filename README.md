# Nymelo 🎵

Turn a name into a tiny, playable melody.

## Run it locally
1. Download and unzip the project.
2. Open `index.html` in Chrome, Edge, Firefox, or Safari.
3. Type a name and press **Make my melody**.
4. Press **Play my melody**. Your browser generates the sound with the Web Audio API.

No build tools, frameworks, account, or API key required.

## Publish free with GitHub Pages
1. Sign in to GitHub and create a new **public** repository named `nymelo`.
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for the published URL shown in the Pages section. It will usually look like `https://YOUR-USERNAME.github.io/nymelo/`.

## What this MVP does
- Converts letters into a repeatable note pattern.
- Generates soft plucked tones in the browser using the Web Audio API.
- Animates the note bars while the tune plays.
- Supports mobile layouts, a tempo slider, sharing a name-specific link, and downloading melody data as JSON.
- Creates a personalised 1080 × 1350 PNG melody card designed for Instagram Stories/posts. Download it or share it where the browser supports image sharing.

## Current limitations / next upgrades
- This is a playful name-to-melody experiment.
- The JSON download saves note data, not an audio recording.
- The melody card is a static image and does not contain playable audio. Use the share-link feature to let people open and play the tune.
- Next possible upgrades: audio export, chord backing, custom melody themes, and a social-ready video export.
- The same name makes the same tune, so a shared URL recreates the same melody.

## Note on sound
Browsers require a user interaction before audio can start. Tap **Play my melody** to enable sound.


## Melody generation
Nymelo uses a repeatable melody-generation algorithm. It uses a C-major pentatonic note set, mostly stepwise movement, slight rhythmic variation, and a resolved ending note. The same name recreates the same melody.


## Sound styles (v3)
The website now offers three browser-generated sound styles:
- **Music Box** — bright, plucked tones.
- **Soft Piano** — a fuller tone with extra harmonics.
- **Dreamy Synth** — a softer, layered sound with gentle detuning.

These are synthesized sounds, not recordings of real instruments. Select a style and press Play to compare them.


## Personalised melody card (v4)
- A story-friendly 1080 × 1350 PNG card is generated in the browser.
- It includes the entered name, a decorative waveform based on the melody, note names, and the selected sound style.
- **Download melody card** saves the PNG. **Share card** uses the browser/device share sheet when supported; otherwise it falls back to sharing the link or downloading the image.
- The card itself is an image, not an audio file. Share the playable name-specific URL separately so friends can hear the tune.
