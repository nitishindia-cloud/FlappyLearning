# Repository guide

- This is a static, browser-based Flappy Bird neuroevolution demo. There is no backend, package manager, or build step.
- `index.html` loads `Neuroevolution.js` before `game.js`; preserve that order. `game.js` handles the game, rendering, and scoring; `Neuroevolution.js` implements networks and generation selection and breeding. Sprites are in `img/`.
- Run by opening `index.html` in a browser, or serve the repository with `python -m http.server 8000` and open `http://localhost:8000/`.
- There is no automated test suite. After changes, check the browser console and verify that images load, birds move, generations advance, and the speed buttons work. Exercise any behavior affected by the change.
- Keep changes focused and consistent with the existing plain JavaScript style; avoid introducing dependencies or a build system unless requested.
