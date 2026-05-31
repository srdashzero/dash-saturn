# LEGAL.md

Dash Saturn is a desktop application and user interface for managing and launching Sega Saturn games owned by the user.

Dash Saturn does not include BIOS files, games, ROMs, ISOs, CHDs or copyrighted firmware. Users must provide legally dumped BIOS and game media that they own.

## Dash Saturn Native Engine

The public product name is Dash Saturn. The public engine name is Dash Saturn Native Engine.

The current implementation launches a native third-party emulator executable as a subprocess for Sega Saturn emulation. The app does not claim that the Saturn emulation core was written from zero by the Dash Saturn project.

## Mednafen Notice

The distributed native runtime currently includes Mednafen components. Mednafen is free software distributed under its own license terms. Keep the original license, copyright notices and credits with any distribution that includes `mednafen.exe`.

The project is migrating toward `dash-saturn-engine.exe`, a Dash Saturn Native Engine binary based on Mednafen source with controlled patches. That does not remove Mednafen's license obligations. Any modified binary must keep the applicable GPL notices and provide corresponding source access for the exact distributed build.

The bundled license file is located at:

```text
resources/emulation/dash-saturn-engine/COPYING
```

Before any public release, ensure that the corresponding source code offer or source access for the exact bundled Mednafen build is available in compliance with the applicable license.

## Third-party Components

Third-party components are documented in `THIRD_PARTY_NOTICES.md` and in their bundled license files.

## ReShade

Dash Saturn may optionally integrate with ReShade as an experimental external post-processing backend.

ReShade is a third-party open-source post-processing injector created by crosire and contributors.

ReShade is licensed under the BSD 3-Clause License. Some source files may also be available under MIT terms when explicitly stated.

ReShade is not created by, owned by, affiliated with, or endorsed by Dash Saturn or Bruno Brian de Paiva Almeida.

All applicable copyright notices, license terms, and credits are preserved in the project documentation.

If ReShade binaries, source, shaders or presets are redistributed with Dash Saturn, preserve all applicable ReShade license terms, copyright notices and credits. The portable runtime copy should keep a ReShade license file next to the runtime, currently named:

```text
resources/emulation/dash-saturn-engine/ReShade_LICENSE.md
```

## Artwork and Metadata Providers

Dash Saturn can search official provider APIs for artwork and metadata when the user configures their own credentials/API keys and explicitly asks the app to search or apply artwork for a game.

Dash Saturn does not scrape provider websites and does not download provider media automatically. Downloaded artwork remains local to the user's app data folder.

Provider media remains subject to each provider's own terms. ScreenScraper community media may be subject to Creative Commons BY-NC-SA 4.0 where applicable.

## No Legal Advice

This document is project documentation, not legal advice.
