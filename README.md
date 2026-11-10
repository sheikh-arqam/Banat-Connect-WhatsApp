# Banat Connect — WhatsApp-style app (Vercel deploy pack)

This folder contains the WhatsApp-style Banat Connect app as a single
self-contained file: `index.html` (702 KB, all images embedded).
It is the FRESH export of the `banat-connect` preview, version v23
with the login fix: solid cream login card (labels readable on the
brown page), visible pink error for a bad email, and the "Continue
with email" button logs in on click as well as on form submit.
Front page (approved BANAT banner), Chats / Calls lists, working
chat buttons (attach / camera / voice note with audio-picker
fallback, emoji), live class, logout. Static / dummy data only —
no backend sync, no Jitsi, no database; chats, files and voice
notes last for the session only.

## Fastest way to get a live URL (no repo needed)

Arqam is already signed in to Vercel on his own PC.

1. On his PC, open https://vercel.com/new?teamSlug=arqam7
   ("Start Building with Vercel").
2. Drag this WHOLE folder (`banat-connect-whatsapp`) onto the page
   (the "drag and drop your project" area), OR click "choose a file
   or a folder" and pick this folder.
3. Vercel deploys it as a static site. When it says READY / "Deployed
   to Production", open the URL it shows (something like
   `banat-connect-whatsapp-xxxx-arqam7.vercel.app`).
4. Check: front page → Chats list with demo classes → open a chat →
   send a message.

## Alternative: via GitHub (if you want auto-deploys later)

1. Arqam creates a NEW empty repo on GitHub (Muse cannot create
   repos via API), e.g. `Banat-Connect-WhatsApp`, Public, no README.
2. Tell Foji it is ready — Foji pushes this folder's contents to it.
3. In Vercel: New Project → Import Git Repository → pick that repo
   → Deploy. Every later GitHub push then auto-deploys.

## Do NOT

- Do NOT deploy this into the `banat-connect-app` Vercel project
  (that is the brown app) and do NOT push it into the
  `Banat-Connect-App` GitHub repo (that holds the new brown code).
  This WhatsApp app is its own standalone project.
