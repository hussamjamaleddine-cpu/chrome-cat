# Chrome Cat

Chrome Cat is a self-contained audio-reactive 9:16 visualizer. Load a local audio track, optionally add cat images or videos as the character, choose effects and scenes, enter fullscreen performance mode, and record the result when supported by the browser.

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static web server. The app uses browser APIs for local media selection, audio analysis, fullscreen mode, and recording; no build step or backend is required.

## GitHub Pages

This repository is intended to be published directly from the `main` branch and the repository root. The `.nojekyll` marker prevents static hosting from applying Jekyll processing to the single-file app.

## Browser permissions and limitations

Audio, image, and video files are processed locally in the browser. Playback and recording availability depends on browser support for Web Audio, Fullscreen, canvas capture, and MediaRecorder. The app includes fallback status messages when a capability or media file is unavailable.
