# IBCA Website – International Bank of Climate Adaptation

A clean, professional static website for the proposed **International Bank of Climate Adaptation (IBCA)**, based on the Ginyard Global Strategy Team presentation materials.

**Headquarters:** Geneva, Switzerland  
**Focus:** Exclusive climate adaptation financing for LDCs and SIDS

## How to Deploy on GitHub Pages

1. Create a new GitHub repository (e.g. `ibca-website` or `ibca-org`).
2. Upload all files in this folder to the root of the repository (or into a `/docs` folder).
3. Go to **Settings → Pages**.
4. Under "Source", select **Deploy from a branch**.
5. Choose branch `main` (or `master`) and folder `/ (root)` or `/docs`.
6. Click Save. Your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/` within a few minutes.

### Optional: Custom Domain
- Add a `CNAME` file in the root containing your domain (e.g. `www.ibca.int`).
- Configure DNS at your registrar to point to GitHub Pages.

## File Structure

```
ibca-website/
├── index.html          # Homepage
├── about.html          # Identity & Why IBCA
├── mandate.html        # Preamble + Object & Purposes
├── membership.html     # Contributing / Recipient / Non-State
├── governance.html     # Structure + Decision-making
├── powers.html         # Powers + Privileges & Immunities
├── funding.html        # Funding sources
├── contact.html        # Contact page
├── css/
│   └── style.css       # All styles
├── js/
│   └── main.js         # Mobile menu
└── README.md
```

## How to Customise (Personalisation)

### 1. Easy text / content changes
Open any `.html` file in a text editor (VS Code, Cursor, Notepad++) and edit the text inside the tags.  
Examples:
- Change headquarters address
- Update contact email
- Add real member lists later
- Modify the hero subtitle

### 2. Colours & branding
Edit `css/style.css` → look for the `:root` variables at the top:

```css
:root {
  --primary: #0d9488;      /* Main teal */
  --accent: #84cc16;       /* Lime accent */
  ...
}
```

Change the hex values to match your official brand colours.

### 3. Add a real logo
Replace the emoji 🌍 in the `.logo` sections with an `<img src="images/logo.svg" alt="IBCA">` and put your logo file in the `images/` folder.

### 4. Add more pages
Copy an existing page (e.g. `about.html`), rename it, update the navigation links in every file, and fill in new content.

### 5. Advanced customisation
- Add a form (use Formspree or Netlify Forms – free tiers available).
- Multilingual: duplicate pages into `/en/` and `/zh/` folders or use a simple language switcher.
- Switch to a static site generator later (Hugo, 11ty, or Next.js + static export) if you need blogs, CMS, or more complex features.
- For full control and modern performance, you can migrate the content into a Next.js project and host on Vercel or Netlify (still free for most use cases).

### 6. Keep content in sync with the PDF
When the official documents are updated, simply edit the corresponding HTML sections. The structure mirrors the presentation chapters for easy maintenance.

## Local Preview
Open `index.html` directly in a browser, or run a simple local server:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit http://localhost:8000

---

Generated from the IBCA strategy presentation (B2 Climate Helper / Ginyard Global Strategy Team).  
Feel free to extend and professionalise further.
