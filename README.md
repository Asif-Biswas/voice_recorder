## How it works
- Uses the browser's **MediaRecorder API** to capture audio from the microphone.
- **Record** starts/stops recording. **Pause** pauses and resumes via `MediaRecorder.pause()/resume()`. **Play** plays back the last recording. **Erase** clears it. **Save** downloads the audio as a `.webm` file.
- Audio chunks are collected into a `Blob` and played/downloaded via an object URL.

## Limitations
- Requires a modern browser with MediaRecorder support (no IE/legacy).
- Pause/resume depends on browser support; if unavailable, recording stops instead.
- Output format is WebM. Some players may not support it natively.

## Tested browsers
- Google Chrome (Version 144), Mozilla Firefox (Version 147), Microsoft Edge (Version 145)
