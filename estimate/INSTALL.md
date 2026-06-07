# Burch Contracting Estimates — Install Guide

This is a standalone, installable app (a PWA). Once installed it runs in its own
window and works fully offline — useful on job sites with no signal.

## Put it online (one-time setup)

Upload this whole folder to your website host, keeping the files together, e.g. so it lives at:

    https://burchcontracting.com/estimate/

The folder must keep this structure (don't rename or separate the files):

    estimate/
      index.html
      manifest.webmanifest
      sw.js
      icons/  (all the .png files)

> A service worker (the offline engine) only runs over **https://** on a real
> domain. Opening the file directly from email or a USB drive will still work as
> a normal web page, but it won't be installable or offline until it's hosted.

## Install it on your phone

iPhone (Safari): open the page → tap the Share button → **Add to Home Screen**.
Android (Chrome): open the page → tap the menu (⋮) → **Install app** /
**Add to Home Screen**. (You may also see an "Install" banner inside the app.)

You'll get a Burch Contracting icon that launches the app full screen.

## First thing to do

Open **Settings** in the app and:
- Your logo is already built in (header + PDF). Upload a different one only if you want to change it
- Set your default tax %, deposit %, and validity days
- Add your common jobs to the Price Book for one-tap quick add
- Use **Export backup** now and then — your data lives on the phone, so a
  backup file protects you if the phone is lost or the browser data is cleared.

SC Lic. #CLG118679 · (864) 724-4600 · Gray Court, SC
