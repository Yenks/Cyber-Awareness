# Think Before You Scan — GMSA-KNUST Cybersecurity Awareness Landing Page

A mobile-first, single-file landing page created for the **GMSA-KNUST IT & Media Cybersecurity Awareness Month (October 2026)**.

Themed around the classic campus bait: **"Looking for free WiFi? You just scanned a random QR code."** Visitors learn how attackers use tempting labels ("Free WiFi", "Free Data", "Scan to win") to lure students into scanning malicious QR codes, and 5 practical rules to protect themselves.

Features zero external dependencies, no build steps, instant load time, high-contrast dark/light mode support, and privacy-first GoatCounter analytics.

---

## 🚀 Quick Deployment Options

Because this is a completely static, single-file site (`index.html`), it can be deployed in under 2 minutes on any modern static hosting provider.

---

### Option 1: Deploy to Vercel

#### Method A: Drag & Drop (Zero Terminal)
1. Go to [vercel.com](https://vercel.com) and log in.
2. In your dashboard, click **Add New…** > **Project**.
3. If you don't use Git, drag and drop the folder containing `index.html` directly into the Vercel import window.
4. Keep the default settings (Framework Preset: **Other** / Root Directory: `./`).
5. Click **Deploy**. Your live URL (e.g. `your-project.vercel.app`) is ready!

#### Method B: Via Vercel CLI
Run in this directory:
```bash
npx vercel
```
Follow the interactive prompts (use default options) to deploy immediately.

---

### Option 2: Deploy to Netlify

#### Method A: Netlify Drop (Fastest)
1. Visit [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop this folder directly onto the drop zone in your browser.
3. Your site will instantly go live with a custom URL (e.g., `https://random-name.netlify.app`).
4. Go to **Site Configuration** > **Change site name** to give it a custom name like `gmsa-knust-cyber.netlify.app`.

#### Method B: Via Git / Netlify CLI
1. Push this folder to a GitHub repository.
2. In Netlify, click **Add new site** > **Import an existing project** > **GitHub**.
3. Select your repository. Leave the Build Command blank and Publish Directory as `.`.
4. Click **Deploy Site**.

---

### Option 3: Deploy to GitHub Pages

1. Initialize git and push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit of cyber landing page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git push -u origin main
   ```
2. On GitHub, go to your repository's **Settings** tab.
3. In the left sidebar, click **Pages**.
4. Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`.
6. Click **Save**. Within 1–2 minutes, your site will be live at:
   `https://<your-username>.github.io/<your-repo-name>/`

---

## ⚙️ Customization & GoatCounter Setup

### 1. Analytics
The GoatCounter tracking script is already embedded in `<head>`:
```html
<!-- PASTE GOATCOUNTER SCRIPT HERE -->
<script data-goatcounter="https://gmsa-cyber.goatcounter.com/count"
        async src="//gc.zgo.at/count.js"></script>
```
To view live visitor counts, log in to your dashboard at [gmsa-cyber.goatcounter.com](https://gmsa-cyber.goatcounter.com).

### 2. Updating Links
In `index.html`, search for `<!-- SECTION 6: OPTIONAL COLLAPSIBLE LEARN MORE -->` to swap the placeholder `href="#..."` links with your actual GMSA social pages, WhatsApp channels, or campus announcements.
