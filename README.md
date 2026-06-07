# Ashin Chakraborty — Portfolio Website

Personal academic portfolio site. Hosted on GitHub Pages.

---

## How to Host This on GitHub Pages (Step by Step)

### Step 1: Create a GitHub account
1. Go to [github.com](https://github.com) and sign up (if you haven't already).

### Step 2: Create a new repository
1. Click the **+** icon (top-right corner) → **New repository**.
2. Name it exactly: `ashin-chakraborty.github.io`
   - Replace `ashin-chakraborty` with your actual GitHub username.
   - If your username is `ashin123`, name it `ashin123.github.io`.
3. Keep it **Public**.
4. **Do NOT** check "Add a README file" (we already have one).
5. Click **Create repository**.

### Step 3: Upload your files
1. On the new repository page, click **"uploading an existing file"** (the link in the instructions area).
2. Drag and drop **all** these files/folders into the upload area:
   ```
   index.html
   README.md
   assets/
     ├── profile.png
     ├── Ashin_Chakraborty_CV.pdf
     ├── Assembly_Representation_Report.pdf
     ├── Migration_Study.pdf
     ├── Reading_Habits_Brochure.pdf
     └── Public_Toilet_Executive_Brief.pdf
   ```
   **Important:** GitHub's web uploader doesn't support folders directly. You have two options:

   **Option A (Easier — upload in two steps):**
   1. First, upload `index.html` and `README.md` to the root. Click **Commit changes**.
   2. Then click **Add file** → **Upload files** again.
   3. Before uploading, click **Create new file** instead, type `assets/placeholder` as the filename, put anything in the content, and commit. This creates the `assets/` folder.
   4. Navigate into the `assets/` folder, click **Add file** → **Upload files**, and upload all 6 files (profile.png + 5 PDFs). Commit.
   5. Delete the `placeholder` file (click it → pencil icon → three dots → Delete file).

   **Option B (Recommended — use GitHub Desktop):**
   1. Download [GitHub Desktop](https://desktop.github.com/).
   2. Clone your new repository to your computer.
   3. Copy this entire `portfolio` folder's contents into the cloned folder.
   4. In GitHub Desktop, you'll see all the files listed. Write a commit message like "Initial upload" and click **Commit to main**.
   5. Click **Push origin**.

### Step 4: Enable GitHub Pages
1. Go to your repository on github.com.
2. Click **Settings** (tab at the top).
3. In the left sidebar, click **Pages**.
4. Under **Source**, select **Deploy from a branch**.
5. Under **Branch**, select **main** and **/ (root)**.
6. Click **Save**.

### Step 5: Visit your site!
1. Wait 1–2 minutes for GitHub to build.
2. Your site is live at: `https://YOUR-USERNAME.github.io/`
3. If you named the repo something other than `username.github.io`, the URL will be `https://YOUR-USERNAME.github.io/REPO-NAME/`.

---

## Updating the Site Later

- To edit `index.html`: click the file on GitHub → pencil icon → edit → **Commit changes**.
- To replace a PDF: navigate to `assets/`, delete the old file, upload the new one **with the exact same filename**.
- Changes go live within 1–2 minutes of committing.

---

## Using a Custom Domain (Optional)

If you buy a domain like `ashanchakraborty.com`:

1. Go to your repo → **Settings** → **Pages**.
2. Under **Custom domain**, type your domain and click **Save**.
3. In your domain registrar (GoDaddy, Namecheap, etc.), add these DNS records:
   - **A records** pointing to:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - **CNAME record**: `www` → `YOUR-USERNAME.github.io`
4. Check **Enforce HTTPS** in GitHub Pages settings.

---

## File Structure

```
/
├── index.html                          ← Your website (single file)
├── README.md                           ← This file
└── assets/
    ├── profile.png                     ← Your profile photo
    ├── Ashin_Chakraborty_CV.pdf        ← Your CV
    ├── Assembly_Representation_Report.pdf
    ├── Migration_Study.pdf
    ├── Reading_Habits_Brochure.pdf
    └── Public_Toilet_Executive_Brief.pdf
```

## What Was Improved

1. **Mobile hamburger menu** — full-screen overlay navigation on mobile
2. **Contact form** — opens the visitor's email client pre-filled with their message
3. **Clean, organized CSS** — well-structured with comments and CSS variables
4. **Dark mode** — automatic, follows system preference
5. **CV preview section** — inline highlights + download button (no dead link)
6. **Social links** — Twitter/X and LinkedIn in nav and footer
7. **Active nav highlighting** — shows which section you're reading
8. **Image fallback** — shows "AC" initials if profile photo fails to load
9. **Open Graph + Twitter Cards** — rich previews when shared on social media
10. **Better typography** — Instrument Serif + DM Sans, refined color palette
