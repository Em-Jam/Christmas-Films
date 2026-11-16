# Christmas Film Countdown

Your Christmas film sheet as a phone app. It comes loaded with all 64 films (your 62, plus Jingle Bell Heist and The Family Stone from the 2025 form), your tiers, streaming services and every logged watch since 2023.

## Put it online (one-off, about 10 minutes)

The app needs a web address, and GitHub Pages hosts it for free.

1. Sign in to github.com (or make a free account) and create a **new repository** called `christmas-films`. Set it to Public, because free Pages sites need that. Only the app code is public; your film list is stored separately in a private Gist.
2. In the new repo, click **Add file > Upload files** and drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js` and the three `.png` icons. Then commit.
3. Go to **Settings > Pages**. Under "Branch", pick `main` and `/ (root)`, then click Save.
4. After about a minute your app is at `https://YOUR-USERNAME.github.io/christmas-films/`.

## Put it on your phone

- **iPhone:** open the link in Safari, tap Share, then **Add to Home Screen**.
- **Android:** open it in Chrome, tap the menu, then **Add to Home screen** (or **Install app**).

## Turn on posters and new releases (TMDB)

1. Make a free account at themoviedb.org.
2. Go to Settings > API and request a developer key. Personal use is fine.
3. In the app, tap the gear icon, paste the key, then tap **Find posters for 64 films**.

If a film gets the wrong poster, open it and tap **Wrong film? Change match**.

## Sync your phone and laptop

1. On GitHub, create a token at Settings > Developer settings > Personal access tokens > Tokens (classic). Tick only **gist** and set no expiry.
2. In the app's settings, paste the token and tap **Save and sync**. Do this on your phone first.
3. Paste the same token on your laptop. It loads the list from GitHub.

The small dot on the gear icon shows sync status: green means synced, gold means saving, red means a problem (open settings to see what's wrong).

## How the countdown works

- It runs from 15 November to Christmas Day. You can change the start date in settings.
- The order is Undecided first (so they get rated), then Bad but good, Winter Vibe, Christmas Vibe, Top, and Elite on the last nights before the 25th.
- "Bad and Bad" is now **Don't watch again**, and those films are never suggested.
- Films already watched this season are skipped. The plan spreads what's left across the remaining nights, at most 2 a night. If there are too many, the lowest tiers drop off first.
- Within a tier, the films you've rewatched most come first.
- Marking an Undecided film as watched asks you to rate it straight away.
- From 26 December to 5 January it suggests Winter Vibe films instead.

## Years and seasons

- Each season runs from July to June, so a film watched on New Year's Day still counts towards that Christmas.
- **Stats** has a season picker (2026, 2025, 2024, 2023). Each season shows only its own watches, plus a list of what you watched that year.
- To add a watch you forgot to log last year, open the film, tap the year under **Log a watch** (the date changes to 15 December of that year, and you can edit it), then tap **Log it**. It counts towards that year only. This season's stats and countdown don't change.
- A film's watch history is grouped by season.

## Backups

In settings, **Download backup** saves your whole list as a file, and **Restore backup** loads one.
