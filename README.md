# TRÉ NATION — website

Single-page, 3D animated artist site. No build step.

## Publish on GitHub Pages
1. Create a repo (e.g. `trenation`) and upload everything in this folder (keep `.nojekyll`).
2. Settings → Pages → Source: "Deploy from a branch" → `main` / root → Save.
3. Live in ~1 minute at `https://<user>.github.io/<repo>/`.
4. Custom domain: Settings → Pages → Custom domain, then point DNS (CNAME to `<user>.github.io`).

## Settings (top of the script in index.html, `CONFIG`)
- `EMBED` — live YouTube / Spotify / Instagram players (leave `true`).
- `PODCAST_EMBED` — paste a podcast player embed URL to add an audio player.
- `INSTAGRAM_POSTS` — list of post URLs to show specific posts.
- `BEHOLD_FEED_ID` — Behold.so feed ID for an auto-updating grid styled like the site.
- `PODCAST_INSTAGRAM` — Instagram handle shown under the podcast (default `gooddaytre`).
- `AUTOSCROLL_SPEED` — default tour speed (0.33 = 33%); visitors adjust it with the − / + control (remembered in their browser). `AUTOSCROLL_ADAPT` slows down for text-heavy sections and pauses longer at their headings. Add `data-speed="0.8"` to a section to set its pace by hand. `AUTOSCROLL_START` auto-starts the tour after the loader; any scroll, swipe or key stops it.
With no posts or Behold ID set, the gallery shows Instagram's live profile embed for @iamtrenation.

Booking: thevibehigh@gmail.com

## Photos (v2)
Photos of Tré load from his public profiles (Spotify, Apple Music, Linktree, SoundBetter, press).
To use your own copies, put files in an `img/` folder and change the URLs in the `PHOTOS` block
near the top of the script (e.g. `src:'img/tre-portrait.jpg'`). `ORBIT` sets which photos circle the 3D heart.

## Background music
The loading screen offers "Enter with sound": "California (feat. John Baab)" from 2:12, looping, in a
"Now Playing" mini player (YouTube requires its player to stay visible, at least 200x200).
Now plays `audio/california.mp3` (the song trimmed to start at 2:12, looping). Set `MUSIC_FILE:''` to fall back to the YouTube player
(`MUSIC_FILE_START` sets where it begins). `MUSIC:false` turns music off; `MUSIC_VOLUME` sets the level.
