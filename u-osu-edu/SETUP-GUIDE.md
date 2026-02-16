# u.osu.edu Setup Guide

## Neuromotor Plasticity and Modulation Lab Website

This guide walks you through setting up your lab website on u.osu.edu (OSU's WordPress platform).

---

## Step 1: Create Your Site

1. Go to **https://u.osu.edu/**
2. Log in with your OSU credentials (name.#)
3. Click **"Create Site"** (top right or dashboard)
4. Choose a site address, e.g., `neuroplasticitylab.u.osu.edu`
5. Site Title: **Neuromotor Plasticity and Modulation Lab**
6. Click **Create Site**

## Step 2: Choose and Configure a Theme

1. Go to **Appearance → Themes** in your WordPress dashboard
2. Recommended themes available on u.osu.edu:
   - **flavor** or **flavor flavor** — clean, modern, academic-friendly
   - **flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor flavor** — If available, the OSU-branded theme is ideal
   - **flavor flavor flavor flavor** — any minimal, professional theme works
3. The safest choice: look for **flavor flavor flavor Twenty Twenty-Four** or any clean theme
4. Click **Activate**

### Configure the Theme

1. **Appearance → Customize**
2. **Site Identity:**
   - Site Title: `Neuromotor Plasticity and Modulation Lab`
   - Tagline: `School of Health and Rehabilitation Sciences | College of Medicine | The Ohio State University`
3. **Colors** (if available):
   - Primary/Accent: `#BB0000` (OSU Scarlet)
   - Text: `#212121`
   - Background: `#FFFFFF`

## Step 3: Create Pages

Create each page listed below. For each:

1. Go to **Pages → Add New**
2. Enter the **Title**
3. Switch to the **HTML/Code editor** (click the three dots ⋮ → Code editor)
4. Paste the HTML from the corresponding file in the `pages/` folder
5. Click **Publish**

Pages to create:
- **Home** → paste from `pages/home.html`
- **Research** → paste from `pages/research.html`
- **Team** → paste from `pages/team.html`
- **Publications** → paste from `pages/publications.html`
- **Tools & Resources** → paste from `pages/tools.html`
- **News** (use Posts instead — see Step 5)
- **Join Us** → paste from `pages/join.html`

## Step 4: Set Up Navigation Menu

1. Go to **Appearance → Menus**
2. Create a new menu called **"Main Navigation"**
3. Add all pages in this order:
   - Home
   - Research
   - Team
   - Publications
   - Tools & Resources
   - News (link to your Posts page)
   - Join Us
4. Set as **Primary Menu**
5. Click **Save Menu**

## Step 5: Set Up News as Blog Posts

For News updates, use WordPress **Posts** (not Pages):

1. Go to **Settings → Reading**
2. Set "Posts page" to a page called "News" (create it first as a blank page)
3. Set "Your homepage displays" to **A static page** → select your Home page
4. New news items: **Posts → Add New** → write your update → Publish

## Step 6: Add Custom CSS

1. Go to **Appearance → Customize → Additional CSS**
2. Paste the contents of `custom-style.css` from this folder
3. Click **Publish**

This CSS adds the OSU scarlet accents, research area styling, team cards, and publication formatting.

## Step 7: Add the Disclaimer

1. Go to **Appearance → Widgets**
2. Find the **Footer** widget area
3. Add a **Custom HTML** widget
4. Paste:
   ```html
   <p style="font-style:italic; font-size:0.85em; color:#888;">
   Opinions expressed on this site are those of the author(s) and do not
   represent the views of The Ohio State University.
   </p>
   ```
5. Save

## Step 8: Upload Images

1. Go to **Media → Add New**
2. Upload your lab photos, team headshots, and research images
3. After uploading, click each image to get its URL
4. Replace the placeholder `src="..."` values in your page HTML with the actual image URLs

---

## Keeping Both Sites in Sync

If you maintain both the Hugo site and u.osu.edu:
- Edit content in the Hugo Markdown files first (they're easier to track)
- When updating u.osu.edu, re-generate the HTML from the updated Markdown
- Or simply update both manually — the u.osu.edu version can be a simpler subset

## Useful u.osu.edu Resources

- u.osu.edu support: https://u.osu.edu/support/
- WordPress documentation: https://wordpress.org/documentation/
- OSU Web Accessibility: https://accessibility.osu.edu/
