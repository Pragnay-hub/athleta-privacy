# Athleta privacy policy — hosting

Google Play will not accept a submission for a location app without a publicly
reachable privacy policy URL. This folder is that page, ready to publish.

`index.html` is a copy of `../athleta-privacy-policy.html`. Edit the source and
re-copy, so the two do not drift.

## Why a separate repo

The main `athleta` repo is **private**. GitHub Pages only serves from a private
repo on a paid plan, so the policy needs its own small public repo. Nothing
sensitive is in it — it is a document written to be read by the public.

## Steps (about 3 minutes)

1. Create a new **public** repo on GitHub named `athleta-privacy`.
   Do not add a README; this folder already has one.

2. From this folder, push it:

   ```bash
   cd store/policy-site
   git init
   git add -A
   git commit -m "Athleta privacy policy"
   git branch -M main
   git remote add origin https://github.com/<your-username>/athleta-privacy.git
   git push -u origin main
   ```

3. In that repo: **Settings → Pages → Source: Deploy from a branch →
   Branch: `main` / `root` → Save.**

4. Wait a minute or two, then open:

   ```
   https://<your-username>.github.io/athleta-privacy/
   ```

5. Put that URL into:
   - Play Console → Store listing → **Privacy policy**
   - `../athleta-play-store-listing.md` (replace the placeholder line)

## Updating it later

Edit `../athleta-privacy-policy.html`, copy it over `index.html`, commit and push.
Change the "Last updated" date whenever the substance changes.
