<img width="1080" height="2400" alt="10" src="https://github.com/user-attachments/assets/b235f224-cfc4-4c86-bf22-0597b3fbdb9b" />
<img width="1080" height="2400" alt="9" src="https://github.com/user-attachments/assets/09a62870-0108-4f38-8b26-e7bc8fab8494" />
<img width="1080" height="2400" alt="8" src="https://github.com/user-attachments/assets/e7f6ff80-2e5c-40d5-bbc3-6a02d3213bf3" />
<img width="1080" height="2400" alt="7" src="https://github.com/user-attachments/assets/66733530-6fdc-4ac0-8ac9-3472f804cecb" />
<img width="1080" height="2400" alt="6" src="https://github.com/user-attachments/assets/6ce16391-68c7-42cf-be00-1dd4bc0751d8" />
<img width="1080" height="2400" alt="5" src="https://github.com/user-attachments/assets/b5582dfd-fb7e-47a5-94b6-fdf090aa574c" />
<img width="1080" height="2400" alt="4" src="https://github.com/user-attachments/assets/f1c50e36-ed26-451a-8e6f-b402a87634b3" />
<img width="1080" height="2400" alt="3" src="https://github.com/user-attachments/assets/2d33ce79-9b8a-4bc8-9bd1-726c698bc6dc" />
<img width="1080" height="2400" alt="2" src="https://github.com/user-attachments/assets/4b948cb9-7222-42cd-babf-d88f6f1f3d49" />
<img width="1080" height="2400" alt="1" src="https://github.com/user-attachments/assets/8792f8e2-1f66-4120-b1d9-6116957138b0" />
<img width="1080" height="2400" alt="0" src="https://github.com/user-attachments/assets/6f2faed7-d98c-4584-9b5d-698a99c3c9bd" />
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
