# THIRD_PARTY_NOTICES.md

Dash Saturn uses third-party software. Do not remove third-party notices from redistributed builds.

## Mednafen

Dash Saturn currently bundles and launches `mednafen.exe` as the native Sega Saturn emulation subprocess behind the Dash Saturn Native Engine.

- Project: Mednafen
- Bundled executable path: `resources/emulation/dash-saturn-engine/mednafen.exe`
- Planned patched engine path: `resources/emulation/dash-saturn-engine/dash-saturn-engine.exe`
- Bundled license path: `resources/emulation/dash-saturn-engine/COPYING`
- Usage in Dash Saturn: subprocess launched by the Electron main process

Mednafen is not authored by the Dash Saturn project. Preserve its license, copyright notices, credits and source availability obligations when distributing builds that include it or a modified Dash Saturn Native Engine derived from its source.

## ffmpeg-static

Dash Saturn uses `ffmpeg-static` to prepare some user-provided disc audio layouts when needed.

Check the package license and bundled notices before public distribution.

## ScreenScraper

Dash Saturn can use the official ScreenScraper API as the primary artwork and metadata provider when the user supplies credentials in the app.

- Website: `https://www.screenscraper.fr`
- Usage in Dash Saturn: user-triggered search/download of Sega Saturn artwork and metadata
- Media storage: `<appData>/games/<gameId>/artwork`

Do not remove provider attribution or ignore provider terms. ScreenScraper community media may be subject to Creative Commons BY-NC-SA 4.0 where applicable.

## TheGamesDB

Dash Saturn can use the official TheGamesDB API as the fallback artwork provider when the user supplies an API key.

- API host: `https://api.thegamesdb.net`
- Usage in Dash Saturn: user-triggered fallback search/download of artwork and metadata
- Media storage: `<appData>/games/<gameId>/artwork`

Provider terms and API limits apply.

## IGDB

IGDB is currently planned for future extra metadata. It is not active in the current provider chain.

## ReShade

ReShade is a generic post-processing injector for games and video software.

- Project: crosire/reshade
- License: BSD 3-Clause
- Copyright: Patrick Mours and contributors
- Local setup source, when present: `reshade-bridge/reshade_utils/opengl32.dll`
- Shader pack path, when present: `reshade-bridge/reshade-shaders`
- Runtime target: `resources/emulation/dash-saturn-engine/opengl32.dll`
- Usage in Dash Saturn: optional OpenGL wrapper/injector for experimental post-processing effects

Dash Saturn may optionally integrate with ReShade as an experimental external post-processing backend. ReShade is third-party software and is not owned by Dash Saturn.

The original license text is preserved in this file or distributed alongside the ReShade components when included.

ReShade is not authored by the Dash Saturn project. If ReShade binaries, source, shaders or presets are redistributed, preserve the applicable license terms, copyright notices and credits. Dash Saturn must not describe ReShade Bridge as native Dash Saturn Engine post-processing.

## Electron and JavaScript Dependencies

Dash Saturn is built with Electron, React, Vite, TypeScript, TailwindCSS, Zustand, electron-store, fs-extra, zod and other npm packages.

Run dependency license review before public distribution.
