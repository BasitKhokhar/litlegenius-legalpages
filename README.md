# Little Genius — Legal Pages

A tiny static website hosting the legal/compliance pages required by Google Play for the
**Little Genius** children's educational app:

- `index.html` — landing / legal center
- `privacy.html` — Privacy Policy
- `terms.html` — Terms & Conditions
- `child-safety.html` — Child Safety Standards (CSAE)
- `data-deletion.html` — Account & Data Deletion instructions

No build step, no dependencies — just static HTML + CSS.

## Deploy to Netlify

### Option A — drag & drop (fastest)
1. Go to https://app.netlify.com/drop
2. Drag this `littlegenius-legalpages` folder onto the page.
3. Netlify gives you a live URL like `https://littlegenius-legal.netlify.app`.
4. (Optional) Rename the site in **Site settings → Change site name**.

### Option B — Git + Netlify
1. Push this folder to its own GitHub repo.
2. In Netlify: **Add new site → Import from Git** → pick the repo.
3. Build command: *(none)* · Publish directory: `.`

## After deploying — wire the URL into the app
Open the app project and edit **`src/Constants/legal.js`**:

```js
export const LEGAL_BASE_URL = 'https://YOUR-SITE.netlify.app';
export const SUPPORT_EMAIL  = 'your-real-support@email.com';
```

Then in the **Google Play Console**, paste these URLs:
- Privacy policy → `https://YOUR-SITE.netlify.app/privacy.html`
- Data deletion (App content → Data safety / Account deletion) → `https://YOUR-SITE.netlify.app/data-deletion.html`
- Child safety standards → `https://YOUR-SITE.netlify.app/child-safety.html`

## Contact (live)
- Developer: **Basit Dev**
- Email: **basitkhokhar957@gmail.com**
- Phone: **03060760549**

## Customise before publishing
- Confirm the effective date (currently **15 June 2026**).
- Contact details across all pages are set to Basit Dev / basitkhokhar957@gmail.com / 03060760549.
