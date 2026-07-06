# amazon-listing-generator

A personal Codex skill for generating and optimizing Amazon listing content.

## What It Does

This skill helps generate or rewrite Amazon listing modules:

- Title
- Bullet Points
- Search Terms
- Product Description in Amazon-compatible HTML format
- Main and secondary image brief
- A+ content brief
- Video script
- Rufus Q&A validation
- Listing self-check

## Custom Rules

- Product Description defaults to HTML format using `<p>` and `<b>` tags.
- Search Terms should avoid repeated words, repeated roots, and repeated meanings as much as possible.
- User-provided facts have priority over common marketplace assumptions.
- Do not invent specs, certifications, compatibility, warranty, safety claims, or compliance claims.

## Install on Another Computer

Copy the `amazon-listing-generator` folder into your Codex skills folder:

```powershell
Copy-Item "amazon-listing-generator" "$env:USERPROFILE\.codex\skills\amazon-listing-generator" -Recurse -Force
```

Then restart Codex.

## GitHub Repo Path

Stored under:

```text
liujingli1233-tech/my-codex-skills/amazon-listing-generator
```
