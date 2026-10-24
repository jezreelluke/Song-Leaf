# Songleaf — standalone app

This is a self-contained web app: your lyric library, plus a scan
feature that reads text out of photos, entirely in your phone's
browser. It doesn't talk to Claude or any server at all — everything
runs and is stored locally on your device.

To install it as a real app on your phone (with its own icon, no
browser address bar, and offline use), it needs to be hosted
somewhere with HTTPS first. Here are three free ways to do that,
easiest first.

## Option 1: Netlify Drop (no account, easiest)

1. Go to **https://app.netlify.com/drop** in a browser on your computer.
2. Drag this whole folder (`songleaf-app`, with all 6 files inside it)
   onto the page.
3. Netlify gives you a link like `https://random-name-123.netlify.app`.
   That's your app's permanent address.

## Option 2: GitHub Pages (if you already use GitHub)

1. Create a new repository and upload all the files in this folder to it
   (keep them at the root of the repo, not in a subfolder).
2. In the repo's **Settings → Pages**, set the source to the `main`
   branch, root folder.
3. GitHub gives you a link like `https://yourname.github.io/reponame/`.

## Option 3: Vercel

1. Go to **https://vercel.com**, sign up, and choose "Add New Project."
2. Upload this folder (or connect it via GitHub).
3. Deploy — Vercel gives you a `https://your-project.vercel.app` link.

## Installing it on your phone

Once it's hosted, open that link **on your phone**, in Chrome
(Android) or Safari (iPhone):

**Android (Chrome):** you should see a banner or a prompt in the menu
saying "Install app" or "Add to Home screen." Tap it.

**iPhone (Safari):** tap the Share button (square with an arrow), then
scroll down and tap **Add to Home Screen**. iOS doesn't show an
automatic install prompt for web apps — this manual step is required.

Once installed, it opens like any other app — full screen, its own
icon, and no address bar — and your saved songs stay on that phone
even without a connection. Scanning does need an internet connection
the very first time you use it on a device (a few MB of one-time
language data), after which it's cached and works offline.

## A note on your data

Everything you save lives in this browser's local storage on this one
device. It is not synced to other devices or backed up anywhere. If
you want your songbook on more than one phone, you'd currently need
to import it on each device separately (or let me know — a shared,
synced version is possible too, just a different kind of build).
