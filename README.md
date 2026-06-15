# FCL Supplier Matcher

Façade Creations Limited — AI-powered supplier routing tool.

## Setup (one-time, ~15 minutes)

### Step 1 — GitHub

1. Go to **github.com** and sign in (or create a free account)
2. Click **New repository**
3. Name it: `fcl-supplier-matcher`
4. Set to **Private**
5. Click **Create repository**
6. Click **uploading an existing file**
7. Drag the entire contents of this zip (all folders and files) into the upload area
8. Click **Commit changes**

### Step 2 — Netlify

1. Go to **netlify.com** and sign up with your GitHub account
2. Click **Add new site → Import an existing project**
3. Choose **GitHub** → select `fcl-supplier-matcher`
4. Leave all build settings as default
5. Click **Deploy site**
6. Wait ~1 minute — Netlify gives you a URL like `https://random-name.netlify.app`
7. (Optional) Go to **Site settings → Domain** to set a custom name

### Step 3 — Add your Anthropic API key

1. In Netlify, go to **Site configuration → Environment variables**
2. Click **Add a variable**
3. Key: `ANTHROPIC_API_KEY`
4. Value: your Anthropic API key (starts with `sk-ant-`)
5. Click **Save**
6. Go to **Deploys → Trigger deploy → Deploy site** to apply

### Done ✓

Your app is live. Share the Netlify URL with your team — everyone sees the same shared supplier database.

---

## How it works

- **Supplier database** — stored in Netlify Blobs (cloud storage, shared across all users)
- **AI matching** — Anthropic API called server-side (key never exposed to users)
- **No login required** — anyone with the URL can use it

## Adding more suppliers

Use the **📋 Supplier Database** tab in the app. Changes are saved immediately for all users.
