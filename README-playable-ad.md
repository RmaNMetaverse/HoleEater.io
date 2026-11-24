# Hole Eater MRAID playable

`index.html` is a short playable ad built from the original game. The player drags the hole to eat 25 blocks, then sees an end card with links to [rman.online](https://rman.online) and [RmaNMetaverse on GitHub](https://github.com/RmaNMetaverse). The same links stay visible during play.

## Ad package

Upload `HoleEater-MRAID-playable.zip` to an MRAID-compatible ad platform. It contains `index.html`, `vendor/three.min.js`, and `vendor/cannon.min.js`. The game needs no network requests to run. The host SDK supplies `mraid.js`; it is intentionally absent from the archive. CTA taps use `mraid.open()` in-app and `window.open()` in a regular browser preview.

The ad pauses gameplay when MRAID reports that it is not viewable. Sound starts off and can only be enabled with the sound button. The package is a general MRAID creative; confirm your chosen ad network's size and archive rules before upload.

## Local preview

Serve this folder with a local HTTP server, then open `index.html`. A missing `mraid.js` request in a regular browser is expected because the ad SDK normally provides that bridge.
