# Nutrition — Food Log (PWA)

Only 3 files: `index.html`, `manifest.json`, `sw.js`. No subfolders — this is
so you can do the whole setup from your phone, no laptop needed.

## 1. Get an Anthropic API key (one-time)
1. On your phone, open https://console.anthropic.com/settings/keys in Chrome
2. Sign in, create a key, copy it somewhere safe
3. You'll paste it into the app's Settings (⚙) the first time you log food
4. Usage is billed to your own Anthropic account — food lookups cost a
   fraction of a cent each

## 2. Host the files with GitHub Pages (all from your phone browser)
1. Go to https://github.com and sign in (or create a free account)
2. Tap the **+** icon (top right) → **New repository**
   - Name it anything, e.g. `nutrition-app`
   - Set it to **Public**
   - Tap **Create repository**
3. On the new repo page, tap **"Add file" → "Upload files"**
4. Tap the upload area to open your file picker, select all 3 files
   (`index.html`, `manifest.json`, `sw.js`) and upload them
5. Scroll down, tap **Commit changes**
6. Go to the repo's **Settings** tab → **Pages** (left sidebar)
7. Under "Build and deployment", set Source to **Deploy from a branch**,
   branch **main**, folder **/ (root)** → **Save**
8. Wait ~1 minute, then refresh — GitHub will show your live URL, something
   like `https://yourusername.github.io/nutrition-app/`

## 3. Install on your phone
1. Open that URL in **Chrome**
2. Tap the ⋮ menu → **"Add to Home screen"**
3. It installs with its own icon and opens full-screen, like a real app
4. Tap ⚙ inside the app and paste your API key — you're set

## Notes
- Your food log and API key are stored only on your phone (localStorage) —
  nothing is lost between sessions, even offline.
- Food lookup itself needs internet; viewing/editing past entries doesn't.
- To update the app later: edit a file on GitHub (pencil icon) or re-upload
  and commit — the live site updates automatically within a minute.
