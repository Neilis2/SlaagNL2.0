# SlaagNL

An educational web platform for Spanish speakers learning Dutch and preparing for the Dutch civic integration exams (Inburgeringsexamen).

## Tech Stack

- **Frontend:** Pure HTML5, CSS3, and Vanilla JavaScript (no build system)
- **Assets:** Local MP3 audio files, MP4 videos, and images
- **APIs:** Browser Web Speech API for Dutch pronunciation (nl-NL)
- **Backend:** Firebase (configured in js/firebase.js)

## Project Structure

- `/` - Root with main `index.html` dashboard
- `/css/` - Global styles (`styles.css`)
- `/js/` - JavaScript utilities (`firebase.js`, `free-access.js`)
- `/assets/` - Audio, video, and image assets
- `/taal/` - Language learning modules (modulo-0 through modulo-3)
- `/samenleving/` - Dutch society (KNS) modules
- `/examen/` - Exam simulations (KNS, reading, speaking)

## Running the App

The app is served as a static site using Python's built-in HTTP server:

```
python3 -m http.server 5000 --bind 0.0.0.0
```

This runs on port 5000 via the "Start application" workflow.

## Deployment

Configured as a static deployment with `publicDir: "."`.
