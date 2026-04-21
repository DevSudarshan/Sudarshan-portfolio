# 🔥 Sudarshan Patil — SRE Portfolio

A dark, neon orange/yellow cyberpunk-themed portfolio website for a Site Reliability Engineer.

**Live Demo:** `https://YOUR-GITHUB-USERNAME.github.io/sre-portfolio`

---

## 📁 Folder Structure

```
sre-portfolio/
│
├── index.html                        ← Main HTML (entry point)
│
├── assets/
│   ├── css/
│   │   └── style.css                 ← All styles
│   ├── js/
│   │   ├── main.js                   ← Cursor, scroll, nav, modals, form
│   │   ├── three-hero.js             ← Three.js animated background
│   │   └── gallery.js                ← Certificate gallery loader
│   └── images/
│       └── (add your profile photo here if desired)
│
└── public/
    └── certificates/
        ├── manifest.json             ← List of certificate image files
        ├── README.md                 ← Instructions for adding certs
        └── (your certificate images go here)
```

---

## 🚀 Deploy to GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub Repository

1. Go to [github.com](https://github.com) → click **New Repository**
2. Name it: `sre-portfolio`
3. Set it to **Public**
4. Click **Create repository**

### Step 2 — Upload Your Files

**Option A — GitHub Web UI (easiest, no terminal needed)**

1. Open your new repo on GitHub
2. Click **"uploading an existing file"** or drag and drop
3. Upload ALL files, keeping the folder structure intact:
   ```
   index.html
   assets/css/style.css
   assets/js/main.js
   assets/js/three-hero.js
   assets/js/gallery.js
   public/certificates/manifest.json
   public/certificates/README.md
   ```
4. Click **Commit changes**

**Option B — Git CLI (if you have Git installed)**

```bash
# Clone your empty repo
git clone https://github.com/YOUR-USERNAME/sre-portfolio.git
cd sre-portfolio

# Copy all portfolio files into this folder
# (the index.html, assets/, public/ folders)

# Push to GitHub
git add .
git commit -m "Initial portfolio upload"
git push origin main
```

### Step 3 — Enable GitHub Pages

1. In your repo, click **Settings** (top tab)
2. Scroll to **Pages** (left sidebar)
3. Under **Source** → select **Deploy from a branch**
4. Branch: **main** | Folder: **/ (root)**
5. Click **Save**
6. Wait 1–2 minutes → your site is live at:
   `https://YOUR-USERNAME.github.io/sre-portfolio`

---

## 🖼️ Adding Certificate Images

1. Add your certificate image files (JPG/PNG/WEBP) to:
   ```
   public/certificates/
   ```

2. Open `public/certificates/manifest.json` and list each file:
   ```json
   {
     "certificates": [
       {
         "file": "cloud-computing.jpg",
         "name": "Master in Cloud Computing"
       },
       {
         "file": "pyramid-cert.jpg",
         "name": "Pyramid Certified Professional"
       }
     ]
   }
   ```

3. Push to GitHub — the gallery updates automatically.

---

## ✏️ Customizing Content

All content is in **`index.html`** — search for the section you want to update:

| Section        | Search for this in index.html           |
|----------------|-----------------------------------------|
| Hero / Name    | `class="hero-h1"`                       |
| Contact info   | `class="pd-contacts"` or `class="cd"`  |
| Skills         | `class="sk-card"`                       |
| Experience     | `class="tl-item"`                       |
| Projects       | `class="proj-card"` + `modalData` in main.js |
| Certifications | `class="cert-card"`                     |
| Education      | `class="edu-card"`                      |
| Hobbies        | `class="hob-card"`                      |

---

## 🎨 Changing Colors

Open `assets/css/style.css` and edit the CSS variables at the top:

```css
:root {
  --o:  #ff6a00;   /* Main orange */
  --o2: #ff9d00;   /* Mid orange  */
  --y:  #ffd000;   /* Yellow      */
  --r:  #ff1a00;   /* Red         */
  /* ... */
}
```

---

## 🌐 Custom Domain (Optional)

To use a custom domain like `sudarshanpatil.dev`:

1. Buy a domain from Namecheap / GoDaddy / Cloudflare
2. In GitHub Pages settings → add your custom domain
3. At your domain registrar → add a CNAME record pointing to:
   `YOUR-USERNAME.github.io`

---

## 📦 Tech Stack

| Technology     | Purpose                        |
|----------------|--------------------------------|
| HTML5          | Structure                      |
| CSS3           | Styling, animations, variables |
| Vanilla JS     | Interactions, scroll, modals   |
| Three.js r128  | 3D hero background             |
| Google Fonts   | Bebas Neue, Rajdhani, JetBrains Mono |

**No build tools. No npm. No dependencies to install.** Just open `index.html` in a browser and it works.

---

## 📞 Contact

**Sudarshan Patil**
📞 +91 87887 09027
✉ sudarshanpatil9881@gmail.com
