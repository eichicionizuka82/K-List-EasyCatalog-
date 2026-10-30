# K-List-EasyCatalog-
### What is K•List?

**K•List** is a simple, fast and minimal app to catalog your series and movies. No bloat, no ads, just your list.

Built with personal API keys integration: **TMDB, MDBList and Pictorium** for metadata, posters, ratings and fanart.

### Features

- 📚 Personal watchlist / watched / favorites
- 🎬 Detail page with cast, trailer, episodes, suggested titles
- 🔍 Search powered by TMDB
- ⭐ Ratings from TMDB + MDBList
- 🖼️ High-quality posters via Pictorium
- 🎨 Clean dark UI - inspired by modern streaming apps

### External Search Integration

K•List does **NOT** host, provide or link to any video streams.

The app can optionally send the selected title as a search query to external apps already installed on your device, such as **CloudStream** and **Nuvio**, via standard Android Intents.

> Example: `ACTION_SEARCH -> query: "A Killer Paradox"`
> The user is fully responsible for the external apps they have installed and how they use them.

You can add, remove or customize external search providers from Settings.

### Setup

1. Clone the repo
```bash
git clone https://github.com/yourusername/K-List.git
```
2. Open in Android Studio
3. Add your own API keys in Settings > API Keys inside the app:
   - TMDB API Key (https://www.themoviedb.org/settings/api)
   - MDBList API Key (https://mdblist.com/)
   - Pictorium API Key
4. Build & run

No keys are hardcoded. An `env.example` is provided for reference.

### Tech Stack

- Kotlin / Jetpack Compose
- TMDB API, MDBList API, Pictorium
- MVVM + Clean Architecture

### Credits & Attribution

This product uses the TMDB API but is not endorsed or certified by TMDB.
All movie and TV show metadata, posters and images are provided by TMDB, MDBList and Pictorium.

Logo: K• - film strip concept by K•List

### Disclaimer

K•List is a personal cataloging tool. It does not host, store or distribute copyrighted content. All external search integrations are user-configured and rely on third-party apps installed separately. Please respect copyright laws in your country.

### License

MIT License - see LICENSE file.

---

Made with ❤️ for movie lovers.
