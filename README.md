# The Mark Server — OAuth application information

This **public** repository contains the static homepage and privacy policy for a personal, read-only Google Drive archival tool used with the owner's creative writing and worldbuilding project, **The Mark**.

**Do not place The Mark manuscripts, database files, Google OAuth secrets, rclone tokens, or other private materials in this repository.** This repository is independent of RPG1.

## Public site files

- [index.html](index.html) — app homepage
- [privacy.html](privacy.html) — privacy policy

## Publish with GitHub Pages

In GitHub, open **Settings → Pages**, then select:

- **Build and deployment → Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/(root)`

Save and wait for GitHub to report the live published URL.

Expected addresses (verify they load before entering them into Google Cloud):

- Homepage: `https://dickwork.github.io/the-mark-oauth/`
- Privacy policy: `https://dickwork.github.io/the-mark-oauth/privacy.html`

Then return to Google Cloud → The Mark Server → Google Auth Platform → Branding and supply those addresses as homepage and privacy policy links. Google's OAuth configuration may also require domain authorization or proof of domain control; `github.io` is a shared hostname and acceptance is not guaranteed.

## Operational status

The public pages describe the intended implementation. Google Drive OAuth authorization and first successful rclone download have not yet been completed. The OAuth requested scope is `drive.readonly` (read-only access across the authorized Drive); the planned rclone operation will select only The Mark's designated Timeline 4 folder. No Google Drive writes are authorized.

Maintain an independent off-machine backup and test restoration before considering this archive fully protected.
