# K-LIST® — an easy catalog

A minimal, offline-first catalog for the series and movies you watch. It started as a personal tool for Korean dramas, but it works for any series and movie.

No account, no ads, no tracking. Your lists live only on your device.

**Download the Android app (APK):** [k-list.apk](https://github.com/eichicionizuka82/K-List-EasyCatalog-/releases/latest/download/k-list.apk)

## Features

**Your lists**
- Series: Completed, Watching, Priority, On hold, To watch, Dropped, Undecided. Movies: Completed, Priority, To watch, Undecided. A title sits in one list at a time.
- Episode and season progress for series, with a progress bar and quick +/- buttons.
- Personal rating, date added and private notes for every title.
- Multiple profiles (up to 4), each with its own lists, ratings and theme.
- Grid or list view, sorting (recent, A–Z, year, rating, your rating), and a status icon on every poster you already have in a list.
- Statistics: total time and episodes watched.

**Title pages**
- Ratings from TMDB, IMDb (via MDBList) or MyDramaList, with more scores from other services.
- Cast, crew, trailers, genres, networks and studios, collections, suggestions and reviews.
- Tap an actor, creator, network, studio or genre to see their other titles.
- "Available on": streaming platforms from TMDB (data provided by JustWatch).
- "Search": opens the title's search directly in **CloudStream** or **Nuvio**, if you have them installed.
- "Download subtitles": SubSource and Wyzie Subs (with optional translation).
- Poster and landscape customization.

**Browse and discover**
- Ready-made TMDB lists (latest, popular, top rated, upcoming) and your own MDBList lists, with a filter for Korean titles only.
- Explore page, search with filters, and people search.

**Other**
- 12 languages: English, Italian, Spanish, French, German, Portuguese, Hindi, Korean, Indonesian, Turkish, Russian and Japanese
- Themes and custom colors.
- Backup and restore as a JSON file.
- Works offline once installed. Your data never leaves the device, apart from the requests you make to the services below.

## Install

**Android (APK):** download [k-list.apk](https://github.com/eichicionizuka82/K-List-EasyCatalog-/releases/latest/download/k-list.apk) and open it. Android may ask you to allow installs from your browser or file manager. To update, use Settings › Check for updates inside the app.

**As a web app (PWA):** open the app's page in Chrome or Brave, then choose "Install".

## Setup

The app needs your own keys for the services it talks to. They are stored on your device and are included in your backup.

| Service | Needed? | Used for | Where to set it |
|---|---|---|---|
| **TMDB** API key | **Required** | Search, posters, details, cast, trailers, TMDB ratings and lists | Settings › Integrations |
| **MDBList** API key | Optional | Custom lists, IMDb rating and other scores | Settings › Integrations |
| **MyDramaList** instance | Optional | Rating, age rating, crew and cast for Korean titles | Settings › Integrations › MyDramaList |
| **SubSource** API key | Optional | Subtitle downloads | Settings › Integrations |
| **Wyzie Subs** API key | Optional | Subtitle downloads and translation | Settings › Integrations |
| **Pictorium** | Optional | Custom posters | Settings › Integrations |

Get a free TMDB key at [themoviedb.org](https://www.themoviedb.org/settings/api). MDBList, SubSource and Wyzie offer free keys too.

### MyDramaList (self-hosted)

MyDramaList has no official API. K-LIST reads it through [Kuryana](https://github.com/tbdsux/kuryana), an unofficial open-source service, so you run your own copy for free:

1. Create a free GitHub account.
2. Open [github.com/tbdsux/kuryana](https://github.com/tbdsux/kuryana) and choose **Fork › Create fork**.
3. Go to [vercel.com](https://vercel.com) and sign in with your GitHub account.
4. **Add New › Project**, pick your fork from the list (do not paste the address) and press **Deploy**.
5. Copy the address Vercel gives you, for example `https://kuryana-xxx.vercel.app` (no trailing `/`).
6. In the app: Settings › Integrations › MyDramaList, turn it on, paste the address, tap **Test connection** and **Save**.
7. To keep it updated, open your fork on GitHub and use **Sync fork › Update branch**. Vercel rebuilds it automatically.

Without an address, MyDramaList stays off and the app uses TMDB. The data is unofficial, so some titles may be missing or differ.

## Privacy

- No account, no analytics, no ads.
- Lists, ratings and notes are stored locally on your device. Use the backup to move them elsewhere.
- The app contacts only the services you set up (TMDB, MDBList, your MyDramaList instance, SubSource, Wyzie, Pictorium), using your own keys.

## Notes

- K-LIST does not host, stream or provide any video content. The CloudStream and Nuvio buttons only pass a title to those apps, which you install and use separately.
- Subtitles are provided by SubSource and Wyzie Subs. Check the terms of those services.

## Build and run

The whole app is a single file, `index.html` (vanilla JavaScript, data in IndexedDB). To run it, serve the folder with any static web server, for example `python3 -m http.server`, and open it in a browser. The Android APK is the same file wrapped in a WebView app.

## Credits

Created by Aisaka82, powered by Claude AI.

This product uses the TMDB API but is not endorsed or certified by TMDB. Streaming availability data is provided by JustWatch. Ratings and lists may come from IMDb, MDBList and MyDramaList, which are trademarks of their respective owners; K-LIST is not affiliated with any of them.
