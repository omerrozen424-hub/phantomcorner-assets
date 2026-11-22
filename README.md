# PhantomCorner assets

Static files the PhantomCorner app loads through jsDelivr, so they are not served from the app's own host.
Every release is a git tag (`v1`, `v2`, ...); the app loads a pinned tag and falls back to its own copy.

- `voice/` - the coach's recorded lines (mp3) and `manifest.json` (text -> file, durations). Generated with
  Kokoro-82M, voice `am_adam` (Apache-2.0).
- `model/movenet-lightning-4/` - MoveNet SinglePose Lightning v4, TensorFlow.js graph model, unchanged from
  tfhub.dev/google/tfjs-model/movenet/singlepose/lightning/4 (Apache-2.0, Google).

No user data is ever stored here.
