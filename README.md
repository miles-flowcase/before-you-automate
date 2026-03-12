# Before You Automate — Flowcase Guide

Hosted interactive guide for: **"Before You Automate: The Expertise Data Problem Top AEC Firms Are Solving"**

---

## Setup: Go live in 5 minutes with GitHub Pages

### Step 1 — Create a GitHub repo

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **New repository**
3. Name it: `before-you-automate` (or `flowcase-guides` if you want to host multiple)
4. Set to **Public**
5. Click **Create repository**

---

### Step 2 — Upload the file

1. In your new repo, click **Add file → Upload files**
2. Upload `before-you-automate-standalone.html`
3. **Rename it to `index.html`** before or after uploading
   - If after: click the file → click the pencil icon → change the filename at the top to `index.html`
4. Commit the file

---

### Step 3 — Enable GitHub Pages

1. Go to **Settings → Pages** in your repo
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main` / Folder: `/ (root)`
4. Click **Save**

Your guide will be live at:
```
https://YOUR-GITHUB-USERNAME.github.io/before-you-automate/
```
(Takes 1–2 minutes to go live the first time)

---

### Step 4 (optional) — Custom subdomain like `read.flowcase.com`

If you want `read.flowcase.com` instead of the github.io URL:

1. In GitHub Pages settings, enter `read.flowcase.com` under **Custom domain**
2. In your DNS provider (wherever flowcase.com is managed), add a **CNAME record**:
   - Name: `read`
   - Value: `YOUR-GITHUB-USERNAME.github.io`
3. Wait ~10 minutes for DNS to propagate
4. Check **Enforce HTTPS** once the domain is verified

---

## Connecting your Flowcase.com form

### Option A — Redirect on form submit (ungated, immediate access)

In your Webflow form settings, set the **Redirect URL** after submission to:
```
https://read.flowcase.com/before-you-automate
```
or with UTM tracking:
```
https://read.flowcase.com/before-you-automate?utm_source=flowcase-site&utm_medium=form&utm_campaign=bya-guide
```

### Option B — Gated (email the link after signup)

1. Connect your Webflow form to HubSpot / Mailchimp / your email tool via Zapier
2. Set up an automated email that sends the guide link after submission
3. The email CTA button links to the GitHub Pages URL

This approach lets you track who actually reads it vs. just submitted the form.

---

## Updating the guide

To update the content:
1. Edit `before-you-automate-standalone.html` locally
2. Go to your GitHub repo → click `index.html` → click the pencil icon → paste updated content
3. Commit — GitHub Pages republishes automatically within ~1 minute

---

## File summary

| File | Purpose |
|------|---------|
| `before-you-automate-standalone.html` | The complete interactive guide (rename to `index.html` in GitHub) |
| `README.md` | This setup guide |
