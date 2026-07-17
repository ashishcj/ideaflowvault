# Ideaflow Vault - Website Deployment & Maintenance Guide

This is a clean, static, high-performance website workspace for the **Ideaflow Vault** platform (`https://www.ideaflowvault.com`). 

It is built using pure semantic HTML, vanilla CSS (no heavy styling frameworks), and vanilla JavaScript. Performance optimization uses `.webp` image formats to achieve high core web vitals scores.

---

## Folder Structure
```text
├── articles/            # SEO-optimized guide subpages
├── index.html           # Main landing page & settings dashboard
├── about.html           # About Us page
├── contact.html         # Contact page
├── ad-calculator.html   # Ad Revenue Calculator tool
├── niche-research.html  # Niche directory page
├── privacy.html         # Privacy Policy page
├── terms.html           # Terms of Service page
├── styles.css           # Global website stylesheet
├── _redirects           # Redirect rules (e.g., ads.txt redirects)
└── sitemap.xml          # Search Engine indexing sitemap
```

---

## How to Test Locally
Since the website is completely static, you can test it locally by opening the `index.html` file in any web browser, or by serving it using a lightweight local web server:

**Using Python:**
```powershell
python -m http.server 8000
```
Then navigate to `http://localhost:8000` in your browser.

---

## How to Deploy Changes Live
The website is configured with Git and hosted using an automated deployment platform connected directly to the GitHub repository at `https://github.com/ashishcj/ideaflowvault.git`. 

Whenever you push a change to the `main` branch, the live website automatically builds and deploys within a few seconds.

### Step-by-Step Deployment Instructions

1. **Verify Your Local Changes:**
   Ensure everything functions correctly locally before staging your changes.

2. **Stage the Modified Files:**
   Open a terminal in the website project directory and run:
   ```powershell
   git add -A
   ```

3. **Commit the Changes:**
   Write a clear, descriptive commit message:
   ```powershell
   git commit -m "description of changes (e.g., chore: update namecheap affiliate link)"
   ```

4. **Push to the Live Repository:**
   Push the changes to the `main` branch on GitHub:
   ```powershell
   git push origin main
   ```

5. **Live Verification:**
   The hosting platform will detect the push and automatically deploy the updates to `https://www.ideaflowvault.com`. Open the site in your browser after 10-15 seconds to verify.
