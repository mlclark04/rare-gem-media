# Rare Gem Media Website

A clean, custom-built website for Rare Gem Media — Little Rock's creative design and digital agency. Built with HTML/CSS, hosted on GitHub Pages, and designed to be easily editable.

## 📁 File Structure

```
rare-gem-media-github/
├── index.html           # Homepage
├── pricing.html         # Pricing page
├── about.html           # About page
├── contact.html         # Contact page
├── README.md            # This file
└── .gitignore           # Git configuration (optional)
```

## 🚀 Getting Started

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `rare-gem-media` (or whatever you prefer)
3. Choose **Public** (required for GitHub Pages to work)
4. Click "Create repository"

### Step 2: Upload Files to GitHub

**Option A: Using GitHub Web Interface (Easiest)**
1. Go to your new repository
2. Click "Add file" → "Upload files"
3. Drag and drop all files from this folder into the uploader
4. Click "Commit changes"

**Option B: Using Git Command Line**
```bash
git clone https://github.com/YOUR_USERNAME/rare-gem-media.git
cd rare-gem-media
# Copy all files from this folder into the cloned directory
git add .
git commit -m "Initial commit: website files"
git push origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository → **Settings**
2. Scroll down to **Pages** section
3. Under "Source," select **main branch**
4. Click "Save"
5. GitHub will give you a URL like `https://YOUR_USERNAME.github.io/rare-gem-media/`

Your site will be live in 1–2 minutes.

### Step 4: Set Up Custom Domain (Optional)

If you want to use `raregemmedia.com`:

1. Go to your domain registrar (GoDaddy, Namecheap, etc.)
2. Point your domain to GitHub Pages by adding these DNS records:
   - `A` records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record: `your-username.github.io` (for www subdomain)
3. Back in GitHub Settings → Pages → Custom domain, enter `raregemmedia.com`
4. Check "Enforce HTTPS"

[Full GitHub Pages custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

---

## ✏️ Editing Content

All pages are plain HTML files. To edit content:

1. **In GitHub web interface:**
   - Click on the file (e.g., `index.html`)
   - Click the pencil icon (Edit)
   - Make your changes
   - Scroll down and click "Commit changes"

2. **Locally (if using Git):**
   - Edit the HTML file in any text editor
   - Save the file
   - Run: `git add .` → `git commit -m "Updated [page name]"` → `git push`

### Common Edits

**Homepage (index.html)**
- Services text: Search for `"Service"` sections in the HTML
- Pricing links: Update href links if pricing changes
- Any headline or body text: Find and replace the text

**Pricing (pricing.html)**
- Update pricing numbers: Search for `$500`, `$2,500`, `$3,000`, etc.
- Edit service descriptions: Find the service text blocks
- Update retainer descriptions

**About (about.html)**
- Edit the main bio paragraph starting with "After 20 years..."
- Update the five philosophy points

**Contact (contact.html)**
- Email: Replace `hey.maeganclark@gmail.com` with your preferred email
- Form action: Update the Formspree ID after you set it up (see below)

---

## 📝 Setting Up the Contact Form

The contact form uses **Formspree** (free tier available).

### Step 1: Create Formspree Account
1. Go to [formspree.io](https://formspree.io)
2. Sign up with your email
3. Create a new form, set it to receive emails at `hey.maeganclark@gmail.com`
4. Formspree will give you a form ID (looks like `f_abc123def`)

### Step 2: Update Contact Form
In `contact.html`, find this line:
```html
<form
  id="inquiry-form"
  class="contact-form"
  action="https://formspree.io/f/YOUR_FORM_ID"
  method="POST"
>
```

Replace `YOUR_FORM_ID` with your actual Formspree ID. That's it — the form will work.

---

## 🔍 SEO Notes

All pages include:
- Meta descriptions optimized for "Little Rock web designer"
- Open Graph tags for social sharing
- Canonical URLs pointing to `raregemmedia.com`
- LocalBusiness schema (homepage)
- Breadcrumb schema (pricing page)

If you change your domain from `raregemmedia.com`, update the canonical URLs in each file.

---

## 🎨 Making Design Changes

All styling is embedded in each HTML file's `<style>` tag. To make design changes:

1. Open the file in a text editor
2. Find the `<style>` section
3. Edit CSS variables at the top (`:root`) to change colors globally:
   - `--pearl`: Background color
   - `--emerald`: Accent color
   - `--ruby`: CTA button color
4. Save and commit

**Color Palette (current):**
- Pearl (off-white): `#FDFCFA`
- Emerald (green): `#1D6647`
- Ruby (red): `#9B1F30`
- Forest (dark): `#0E3322`

---

## 🚨 Important Notes

- **Keep files in root directory** — GitHub Pages serves files from the root by default. Don't move them into a subfolder.
- **File naming matters** — Use lowercase filenames. `about.html` works; `About.html` might not on some servers.
- **Cache clearing** — Changes usually appear within 1–2 minutes. If you don't see an update, try a hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac).
- **Backup your files** — Keep a local copy of all HTML files as backup.

---

## 📞 Support & Troubleshooting

**Site not showing up after pushing to GitHub?**
- Check that the repository is **Public** (not Private)
- Wait 2–3 minutes for GitHub Pages to rebuild
- Check Settings → Pages to confirm it's enabled and showing the correct branch

**Form not working?**
- Make sure you've updated the Formspree form ID
- Test by filling out the form and checking your email
- Check Formspree dashboard for submission logs

**Pages not linking correctly?**
- All links use relative paths (e.g., `href="pricing.html"`)
- Make sure file names match exactly (case-sensitive on some servers)

**Custom domain not working?**
- DNS changes can take up to 48 hours to propagate
- Verify your DNS records are set correctly
- Check GitHub Pages documentation for your registrar

---

## 🎯 Next Steps

1. ✅ Push files to GitHub
2. ✅ Enable GitHub Pages
3. ✅ Set up Formspree form
4. ✅ (Optional) Point custom domain
5. ✅ Test all links and the contact form
6. ✅ Share with the world

---

**Built with intention. Built to last.**

*Rare Gem Media © 2025*
