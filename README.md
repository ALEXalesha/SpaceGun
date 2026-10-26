<div align="center">

# Space Gun

**Space Gun («Космический стрелок») is a top-down space shooter in a single HTML page: waves of ships and asteroids, bosses and a workshop between sectors. It runs in the browser with no server and no internet: open `index.html` or play it online.**

[**▶ Play online →**](https://alexalesha.github.io/SpaceGun/) &nbsp;·&nbsp; [Русская версия этого файла](README.ru.md)

[![Status](https://img.shields.io/badge/status-stable-brightgreen)](#) [![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE) [![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML) [![Website](https://img.shields.io/badge/Website-open-0A84FF?logo=googlechrome&logoColor=white)](https://alexalesha.github.io/SpaceGun/) [![Built with Claude Code](https://img.shields.io/badge/Built_with-Claude_Code-D97757?logo=claude&logoColor=white)](https://claude.com/claude-code)

Code, tests and docs are written by Claude (Anthropic) in Claude Code. Ideas, testing and decisions - Alexey.

</div>

> Fan-made game. Ships, explosions and nebulae are drawn by code.

The interface is in Russian.

![Menu](docs/screens/menu.png)

![A sector of the campaign](docs/screens/play.png)

![The Core, the last boss](docs/screens/boss.png)

## What is in the game

- **Campaign of 8 sectors:** several waves each, then an elite squadron or a boss (the Warden, the Swarm Mother, the cruiser "Thunder", the Core).
- **Workshop** after a sector: credits buy better weapons, damage, armour, engines and fire rate, repairs and bombs.
- **Survival:** endless waves, the weapon upgrades itself every 3 waves.
- Snipers show their line of fire first, the cruiser and the Core fire beams: leave the line while it is dashed.
- Achievements and records, settings with aim assist, gamepad support; music and sounds are synthesised with WebAudio.

## Controls

| Key | Action |
|---|---|
| WASD or arrows | fly |
| Mouse | aim |
| Left mouse button or Space | fire |
| E | bomb |
| Esc | pause |

Keys can be changed in the settings where the game offers it; a gamepad works too where noted above.

## Run locally

Open `index.html` in Chrome, Edge or Firefox. Everything is in the repository; nothing is downloaded.

## Tests

The laws are Playwright tests in `tests/`. They open the page by its file address in headless
Chromium, one at a time:

```
npm install
npx playwright install chromium
npm test
```

Mouse capture in the tests is always a stub (a real `requestPointerLock` in headless Chromium on
Windows can clip the user's cursor).
The pictures above were made headless by the screenshot script of the Hub collection.

## History

The game was made in the [Hub](https://github.com/ALEXalesha/ALEXalesha.github.io) collection (folder `web/space_shooter`), where it also runs in the Hub ([play there](https://alexalesha.github.io/)). This repository carries the game with its commit history.

## Licence

MIT, see [LICENSE](LICENSE).
