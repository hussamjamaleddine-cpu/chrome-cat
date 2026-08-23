# Chrome Cat

Chrome Cat is a self-contained audio-reactive 9:16 visualizer designed for modern browsers on Android phones, iPhones and iPads, tablets, Windows PCs, and Mac computers. Load a local audio track, optionally add cat images or videos as the character, choose effects and scenes, enter fullscreen performance mode, and record the result when supported by the browser.

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static web server. The app uses browser APIs for local media selection, audio analysis, fullscreen mode, and recording; no build step or backend is required.

## GitHub Pages

This repository is intended to be published directly from the `main` branch and the repository root. The `.nojekyll` marker prevents static hosting from applying Jekyll processing to the single-file app.

## Browser permissions and limitations

Audio, image, and video files are processed locally in the browser. The page uses responsive sizing, safe-area insets, touch-friendly controls, iOS share/download fallbacks, and dynamic viewport handling for phones and tablets. Playback and recording availability depends on browser support for Web Audio, Fullscreen, canvas capture, and MediaRecorder. Mobile browsers may require a manual Play tap because of autoplay policies, and iOS may present a Share flow instead of a direct recording download. The app includes fallback status messages when a capability or media file is unavailable.

Saved image characters are persisted as downscaled JPEG source copies to avoid repeated contrast processing and storage overuse. As a known limitation of this compact archive format, transparent PNG backgrounds are flattened during persistence and may appear with a dark background after reload.

iOS home-screen icon: the favicon is an inline SVG data URI. iOS Safari requires a binary PNG for apple-touch-icon, so adding the app to an iOS home screen shows a screenshot thumbnail rather than the Chrome Cat icon. Not fixed, as it would require committing a binary asset.
