# Aman Shah — personal site

A Jekyll site that GitHub Pages builds and hosts for free. You never need to install anything: everything below happens in the GitHub website.

## Put it online (one time, about 20 minutes)

1. **Create a GitHub account** at github.com if you don't have one. Pick a professional username (for example `amanshah`).
2. **Create a repository** named exactly `<your-username>.github.io` (for example `amanshah.github.io`). Set it to **Public**. Don't add a README.
3. **Upload the files.** On the empty repository page, choose "uploading an existing file". Drag in everything inside this folder, including the `_layouts`, `_data` and `assets` folders, then click **Commit changes**.
4. **Turn on Pages.** Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, and save.
5. After a minute or two the site is live at `https://<your-username>.github.io`.

## Connect amanshah.live

The site is already set up for amanshah.live (the `CNAME` file and the `url` in `_config.yml`).

1. At your domain registrar, open the DNS settings for amanshah.live. Delete any existing "parking" or "forwarding" records for `@` and `www`, then add:
   - Four `A` records, host `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record, host `www`, pointing to `<your-username>.github.io`
2. In GitHub, **Settings → Pages → Custom domain**, enter `amanshah.live` and save.
3. Once the DNS check passes (usually under an hour, up to a day), tick **Enforce HTTPS**.
4. Optional but recommended: verify the domain under your GitHub account's **Settings → Pages** (the account settings, not the repository), so no one else can claim it.

## Publish an article

1. In the repository, open the `_posts` folder (if it doesn't exist yet, it will be created by step 2).
2. Click **Add file → Create new file**. Name it `_posts/YYYY-MM-DD-short-title.md`, for example `_posts/2026-11-20-ptp-boundary-clocks.md`. The date in the name is the publish date.
3. Paste this at the top, fill it in, and write the article below the second `---`:

```markdown
---
layout: post
title: "PTP in Practice: Boundary Clocks and Grandmaster Failover"
summary: "One or two sentences shown in the article list and in link previews."
topics: [PTP, SMPTE ST 2059-2, ST 2110]
# If the article first appeared elsewhere, fill these in; otherwise delete both lines.
venue: "TV Technology"
venue_url: "https://www.tvtechnology.com/..."
---

Opening paragraph.

## A section heading

- A list item
- **Bold**, *italic*, `code`, and [a link](https://example.com)
```

4. Click **Commit changes**. The article is live within a couple of minutes.

To edit or delete an article later, open its file in `_posts` and use the pencil (edit) or trash icon.

**Keep drafts off GitHub.** A public repository shows every file, so write drafts elsewhere and only add the file when it's ready to publish.

## Add a talk or publication

Edit `_data/pubs.yml` and add an entry at the top, following the ones already there. Keep the two-space indentation.

## Change profile text

The profile, selected work and experience sections are in `index.html`. Edit the text between the tags and commit.

## For the EB-1A file

- Republish each trade or journal article here with `venue` and `venue_url` filled in, so the site works as a dated index of your bylined work.
- Save a PDF of the site and of each article page when you file, since the officer sees the evidence as it was on the filing date.
- Get Arista PR/legal sign-off before posting work-related content.
