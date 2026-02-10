<p align="center">
    <a href="https://gamemaker.io/"><img src="https://github.com/bytecauldron/awesome-gamemaker/raw/main/images/banner.png" /></a>
</p>

# Awesome GameMaker [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Made with GameMaker](https://img.shields.io/badge/Made%20with-GameMaker-000000.svg?style=flat\&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAAAZlBMVEX%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2BrG8stAAAAIXRSTlMABg0OFBkfcn1%2Bf4CBgoOFhoeIiouWmNDa5ebp8PX2%2B%2F6o6Vq%2BAAAAY0lEQVR42k2OWQ6AIAwFn%2BIOioobrnD%2FS4o0EeanmQxNAdErRFTWtsFq6%2BiiZozz0CSnTjYBwo0RkF8DWDLf51Ni9K%2FYdq0Fy3KAfzk97M7goK1F%2F4rGH9Kk1OlboQtEDIrmC%2BU3CVxTr%2FRMAAAAAElFTkSuQmCC)](https://www.yoyogames.com/gamemaker) [![Links](https://github.com/bytecauldron/awesome-gamemaker/actions/workflows/links.yml/badge.svg)](https://github.com/bytecauldron/awesome-gamemaker/actions/workflows/links.yml) ⭐ 443 | 🐛 1 | 📅 2026-01-08 with stars

> A curated list of awesome libraries, snippets, guides, and projects for GameMaker. 😎

[GameMaker](https://gamemaker.io/) is a user-friendly, cross-platform game engine by YoYo Games that allows both beginner and advanced game developers to create 2D and 3D games for desktop, HTML5, and console platforms.

What kind of games can you make in GameMaker? [Check out this list.](https://steamdb.info/tech/Engine/GameMaker/)

## Contents

* [Getting Started](#getting-started)
* [Data Manipulation](#data-manipulation)
* [Native Extensions](#native-extensions)
* [Timing](#timing)
* [Utilities](#utilities)
* [Tools](#tools)
* [Debugging](#debugging)
* [Input Handling](#input-handling)
* [User Interface](#user-interface)
* [Localization](#localization)
* [Physics](#physics)
* [Sprites](#sprites)
* [Audio](#audio)
* [Levels](#levels)
* [Particles](#particles)
* [Lighting](#lighting)
* [Shaders](#shaders)
* [3D](#3d)
* [Sprite Stacking](#sprite-stacking)
* [Networking](#networking)
* [Integrations](#integrations)
* [Camera](#camera)
* [Sequences](#sequences)
* [State Machines](#state-machines)
* [Pathing](#pathing)
* [Useful Extras](#useful-extras)
* [Blogs](#blogs)
* [YouTube](#youtube)
* [Community](#community)
* [Special Thanks](#special-thanks)

## Getting Started

* [GameMaker Manual](https://manual.gamemaker.io/)
* [GameMaker Release Notes](https://gms.yoyogames.com/ReleaseNotes.html)
* [GameMaker Marketplace](https://marketplace.gamemaker.io/)
* [Beginner GameMaker Tutorials](https://www.youtube.com/watch?v=nBCDzE9MDbk\&list=PLPRT_JORnIur4v19PHXCtJ5P05vaokFdP) - Tutorials from Shaun Spalding. A comprehensive introduction to basic features of the IDE. Highly recommended to check out the full playlist if you're a complete beginner. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Advanced GameMaker Tutorials](https://www.youtube.com/watch?v=n8-MuIuOQFE\&list=PL_hT--4HOvrfuDcYrTufdpgwoALAczPR2) - Tutorials from DragoniteSpam that dive into more advanced topics related to the GML language. They also have comprehensive 3D and shader introduction videos. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)

### Recommendations

* If you already have programming experience, learn the GameMaker Language (GML) instead of the Visual (Drag and Drop) feature.
* For pixel art, [Aseprite](https://www.aseprite.org/) is a popular alternative to the native sprite editor. 💸
  * [Aseprite's source code](https://github.com/aseprite/aseprite) ⭐ 35,632 | 🐛 1,900 | 🌐 C++ | 📅 2025-12-30 can be compiled for free.
* Don't be afraid to use other developer libraries. A lot of them are free for a reason. Just be mindful of the license.
* Updates to the IDE and runtime can break your game (like syntax changes to GML). If you are working in a group, make sure you are running on the same version of GMS and only update when given a fair warning. You can reinstall previous versions of your IDE at the GMS download page.
* Unless your game requires complex physics interactions, it's generally advised to avoid GameMaker's built-in physics system.
* Schedule routine backups for projects. If you are dealing with larger media files in your repo, try [Git LFS](https://git-lfs.github.com/).

## Data Manipulation

This includes data structures and file formats that do not fit into a more specific category.

* [SNAP](https://github.com/JujuAdams/SNAP) ⭐ 95 | 🐛 5 | 🌐 Game Maker Language | 📅 2026-01-19 - Easy data format saving and loading. Please note that newer versions of GameMaker contain `json_parse` and `json_stringify`. However, if you are converting csv, ini, xml, etc, you may find this very useful.
* [OKColor](https://github.com/KeeVeeGames/OKColor.gml) ⭐ 47 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-18 - An okay color manager for implementing OKLab/OKLCH colors.
* [GML-OOP](https://github.com/Mtax-Development/GML-OOP) ⭐ 32 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-21 - A constructor library for operating the primary functionalities of GameMaker.
* [ForEach](https://github.com/KeeVeeGames/foreach.gml) ⭐ 26 | 🐛 0 | 🌐 Game Maker Language | 📅 2020-10-13 - Adds a foreach implementation for arrays, ds\_lists, ds\_maps, ds\_stacks, ds\_queues, ds\_priorities and structs.
* [Destructors](https://github.com/DatZach/Destructors) ⭐ 25 | 🐛 2 | 🌐 Yacc | 📅 2022-10-24 - Allows you to use ds\_\* types such as lists and maps inside of structs.
* [Promises](https://github.com/YAL-GameMaker/Promise.gml) ⭐ 25 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-07-21 - An adaptation of JavaScript Promises.
* [ArrayList](https://github.com/KeeVeeGames/ArrayList.gml) ⭐ 18 | 🐛 0 | 🌐 Game Maker Language | 📅 2020-12-03 - The most complete list class. Garbage collected, fast sort function, \[] accessor and referencing as an array.
* [Exception](https://github.com/KeeVeeGames/Exception.gml) ⭐ 17 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-03-29 - A base class for custom exceptions.
* [GML-Classes](https://github.com/Nikko-the-cat/GML-Classes) ⭐ 15 | 🐛 0 | 🌐 Yacc | 📅 2024-05-08 - Another project that adds OOP functionality to GameMaker.
* [Cottonwool](https://github.com/JujuAdams/Cottonwool) ⚠️ Archived - Safe surfaces without memory leaks.
* [DeepCopy](https://github.com/KeeVeeGames/DeepCopy.gml) ⭐ 12 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-03-18 - Deep clone class instances / constructed structs, anonymous structs and arrays nested in any order!
* [LWO](https://github.com/tabularelf/lwo) ⚠️ Archived - Lightweight objects using structs.
* [Lock And Key](https://github.com/AlubJ/Lock-And-Key) ⭐ 9 | 🐛 0 | 🌐 Yacc | 📅 2020-09-07 - String and file encryption.
* [gm-stream](https://github.com/daikon-games/gm-stream) ⭐ 8 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-03-02 - Data structure manipulation.
* [Matrices](https://github.com/JujuAdams/matrices) ⭐ 6 | 🐛 3 | 🌐 Game Maker Language | 📅 2024-02-18 - A collection of matrix handling scripts.
* [BSONGML](https://github.com/LAGameStudio/BSONGML) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-03-22 - Save and load GML structured data in binary files, skirting memory and performance concerns associated with loading JSON as a string.
* [Binder](https://github.com/Homunculus84/Binder) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-06-19 - A binary search library for efficient lookups on large datasets.
* [Map](https://github.com/GameMakerDiscord/Map.gml) ⭐ 3 | 🐛 0 | 🌐 HTML | 📅 2020-06-14 - Hash table implementations.
* [Airkiver](https://github.com/AlubJ/Airkiver) ⭐ 1 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-20 - Game file archive tool.
* [Ngrams](https://github.com/tinkerer-red/Ngrams) ⭐ 1 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-10 - Lightweight n-gram library for fuzzy search, predictive text or token sequence modeling.
* [Bit Buffers](https://yellowafterlife.itch.io/gamemaker-bit-buffers) - Read and write buffers with per-bit granularity.
* [sprite\_add\_gif](https://yellowafterlife.itch.io/gamemaker-sprite-add-gif) - Dynamically load animated GIFs as sprites.
* [Managix](https://foxyofjungle.itch.io/managix) - Async memory & resources manager (texture groups, audio groups, etc). 💸

## Native Extensions

These work on specific platform(s) and enable the games to do something that would be impossible, impractical, or inefficient to do in GML alone. Native extensions related to a specific task (e.g. input handling) can be found in those sections.

* [GMD3D11](https://github.com/blueburncz/GMD3D11) ⭐ 29 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-17 - A DLL for interfacing with Windows Direct3D.
* [GMSDLL](https://github.com/YAL-GameMaker/GMSDLL) ⭐ 18 | 🐛 0 | 🌐 C++ | 📅 2024-06-15 - A template project for building DLLs for GameMaker.
* [wasm-bridge](https://github.com/Sidorakh/wasm-bridge) ⭐ 15 | 🐛 0 | 🌐 JavaScript | 📅 2025-08-28 - A way to use JS extensions in GX/WASM games.
* [gameframe](https://github.com/YAL-GameMaker/gameframe) ⭐ 14 | 🐛 0 | 🌐 Haxe | 📅 2024-09-15 - Custom window caption and border for Windows.
* [GM Sysinfo](https://github.com/SpikeHD/gm-sysinfo) ⭐ 11 | 🐛 1 | 🌐 Rust | 📅 2023-12-12 - Cross-platform extension for getting system information and resource usage.
* [GMSDLL.rs](https://github.com/YAL-GameMaker/GMSDLL.rs?) ⭐ 6 | 🐛 0 | 🌐 Rust | 📅 2025-09-14 - Example on how to make native DLL extensions in Rust.
* [file\_dragger](https://github.com/YAL-GameMaker/file_dragger) ⭐ 5 | 🐛 0 | 🌐 Batchfile | 📅 2024-06-11 - Drag-and-drop files *out* of the game window on Windows.
* [zlib functions](https://yellowafterlife.itch.io/gamemaker-zlib) - Simple compression/decompression functions.
* [Window Taskbar](https://yellowafterlife.itch.io/gamemaker-window-taskbar) - Windows only. Flash the game window border and/or its taskbar button.
* [Extension Collection](https://samuel-venable.itch.io/gamemaker-extension-collection) - A suite of various extensions.
* [Video Player Extension](https://forum.yoyogames.com/index.php?threads/video-player-for-windows-macos-and-ubuntu.77882/) - Play videos. However, the latest version of GMS has video support.
* [GMESCAPI](https://marketplace.yoyogames.com/assets/9529/gmescapi) - Webcam capture.
* [Rousr Release](https://gitlab.com/rousr-release/) - Unmaintained projects from the Rousr team (in case anyone asks where OutsideTheBox/Dissonance went).
* [window\_shape](https://yellowafterlife.itch.io/gamemaker-window-shape) - Custom-shaped windows on Windows. 💸
* [Windows' windows](https://yellowafterlife.itch.io/gamemaker-winwin) - Multiple windows on Windows. 💸
* [winMenu](https://yellowafterlife.itch.io/gamemaker-winmenu) - Native menus on Windows. 💸
* [window\_set\_icon](https://yellowafterlife.itch.io/window-set-icon) - Change window and/or taskbar icons on Windows.
* [file\_dropper](https://yellowafterlife.itch.io/gamemaker-file-dropper) - Accept drag-and-dropping files onto a game window on Windows.
* [Window Commands](https://yellowafterlife.itch.io/gamemaker-window-commands) - Dispatch/intercept window controls like Minimize (and other window-related functions).
* [Web Dynamic Textures](https://yellowafterlife.itch.io/gamemaker-web-dyn-textures) - A dynamic texture page loading system for HTML5.
* [GMWinBackdrop](https://topherlicious.itch.io/gmwinbackdrop) - Windows 11 backdrop materials.

## Timing

Custom timers, timelines, and task scheduling.

* [Iota](https://github.com/JujuAdams/iota) ⭐ 47 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-10-20 - Lightweight timestep library.
* [fuwafuwa](https://github.com/kemonologic/fuwafuwa) ⭐ 6 | 🐛 10 | 🌐 Game Maker Language | 📅 2022-07-28 - Easy-to-use timer system.
* [GMTimeLine](https://github.com/TimVN/GMTimeLine) ⭐ 6 | 🐛 0 | 🌐 Yacc | 📅 2022-11-03 - A pure code alternative to GameMaker timelines.
* [Stopwatch](https://github.com/Lojemiru/Stopwatch) ⭐ 4 | 🐛 0 | 🌐 Yacc | 📅 2022-10-28 - GameMaker alarm replacement.
* [FrogAlarm](https://github.com/colmeye/FrogAlarms) ⭐ 3 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-03-26 - Another easy alternative to GameMaker alarms.
* [Timer](https://github.com/nommiin/Timers) ⭐ 3 | 🐛 0 | 🌐 Yacc | 📅 2020-04-24 - Timer methods based on setTimeout and setInterval from JS.
* [Agenda](https://github.com/benal20/Agenda.gml) ⭐ 3 | 🐛 2 | 🌐 Yacc | 📅 2023-07-01 - Schedule and delay the execution of callbacks.
* [wTimer](https://mors-games.itch.io/wtimer) - Robust alternative for alarms.

## Utilities

* [Catspeak](https://github.com/katsaii/catspeak-lang) ⭐ 121 | 🐛 8 | 🌐 Game Maker Language | 📅 2025-11-20 - Cross-platform programming language for modding support.
* [Coroutines](https://github.com/JujuAdams/Coroutines) ⭐ 82 | 🐛 3 | 🌐 Game Maker Language | 📅 2025-06-29 - Asynchronous functions for GameMaker.
* [handytools](https://github.com/JujuAdams/handytools/) ⚠️ Archived - A collection of Juju's libraries in one convenient project.
* [SSave](https://github.com/stoozey/SSave) ⭐ 39 | 🐛 10 | 🌐 Game Maker Language | 📅 2025-10-13 - Simple file saving system.
* [DDDEditor](https://github.com/DragoniteSpam/DDDEditorGMS2) ⭐ 33 | 🐛 7 | 🌐 Game Maker Language | 📅 2026-01-22 - General purpose game editor.
* [Dynamo](https://github.com/JujuAdams/Dynamo) ⭐ 33 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-26 - Dynamic data loader.
* [FAST](https://github.com/Hyomoto/FAST) ⭐ 32 | 🐛 1 | 🌐 Game Maker Language | 📅 2022-01-10 - Flexible Assistant Toolkit. Similar to gm-core but comes with input and resolution handling.
* [GMBenchmark](https://github.com/DragoniteSpam/GMBenchmark) ⭐ 31 | 🐛 2 | 🌐 Game Maker Language | 📅 2025-08-30 - A tool to benchmark GML code.
* [Seedpod](https://github.com/daikon-games/gm-seedpod) ⭐ 28 | 🐛 1 | 🌐 Game Maker Language | 📅 2023-07-18 - A collection of scripts to improve the GML programming experience.
* [GMLodash](https://github.com/DatZach/GMLodash) ⭐ 24 | 🐛 1 | 🌐 Game Maker Language | 📅 2021-11-28 - Functional programming in GML.
* [Figgy](https://github.com/glebtsereteli/Figgy) ⭐ 22 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-28 - Centralized and persistent live configs for seamless game tuning and balancing.
* [Canvas](https://github.com/tabularelf/Canvas) ⭐ 19 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-31 - Another great solution for surface management.
* [Mathematical Scripts](https://github.com/adam-rumpf/game-maker-scripts) ⭐ 17 | 🐛 1 | 🌐 Game Maker Language | 📅 2023-06-12 - A collection of math scripts.
* [Broadcast](https://github.com/JulianDicken/Broadcast) ⚠️ Archived - Event handling library.
* [GameMaker Scaffolding](https://github.com/babaganosch/GameMakerScaffolding) ⭐ 13 | 🐛 0 | 🌐 Yacc | 📅 2023-12-28 - Another cool all-encompassing template with a focus on building low-res, tile-based games.
* [Polarca](https://github.com/VitorEstevam/polarca) ⭐ 11 | 🐛 1 | 🌐 Game Maker Language | 📅 2024-03-11 - Interpolation functions.
* [Gumshoe](https://github.com/JujuAdams/Gumshoe) ⭐ 11 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-03-04 - Simple deep file search function.
* [CoreExtension](https://github.com/blueburncz/CoreExtension) ⚠️ Archived - A collection of CC0 programming libraries. (archived)
* [Autoframer](https://github.com/mstop4/auto-framer) ⭐ 7 | 🐛 0 | 🌐 Yacc | 📅 2021-05-02 - Automatically handles resizing the game view across different display and window sizes.
* [gml-highscorer](https://github.com/Grisgram/gml-highscorer) ⭐ 7 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-09-01 - Highscore and trophy system.
* [RenderStack](https://github.com/FoxyOfJungle/RenderStack) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-17 - Organize your game's rendering into a customizable order.
* [Voxeledphoton's FreeGMScripts](https://github.com/vphoton/FreeGMScripts) ⭐ 3 | 🐛 0 | 📅 2023-01-10 - Additional GML helper functions. Some may be out of date with 2.3+ syntax.
* [JITSpeak](https://github.com/BenjaminUrquhart/JITSpeak) ⭐ 3 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-11-08 - Improves Catspeak performance.
* [GML-Multiprocessing](https://github.com/tinkerer-red/GML-Multiprocessing) ⭐ 1 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-10-09 - A proof of concept for multiprocessing.
* [gm-core](https://github.com/gm-core) - Foundational utility suite and a great starting point for new GameMaker projects. Comes with quality of life methods, networking tools, testing framework, delta timing, and more.
* [Twerp](https://pixelatedpope.itch.io/twerp) - Easing function similar to lerp().
* [Trixscript](https://trixelized.itch.io/trixscript) - Juices up your game with useful functions.
* [Motion Scripts](https://avis.itch.io/motion-scripts) - Provides replacement methods for built-in motion variables.
* [GML+](https://xgasoft.itch.io/gmlp) - A script collection with a goal to "fill the gaps" in GML. 💸
* [GMLive](https://yellowafterlife.itch.io/gamemaker-live) - Livecoding / interactive programming. 💸

## Tools

Things that work with project files or GameMaker itself rather than being something that's used in-game.

* [GMEdit](https://github.com/YellowAfterlife/GMEdit) ⭐ 358 | 🐛 24 | 🌐 JavaScript | 📅 2026-01-25 - Code editor to use in conjunction with GameMaker.
* [Rubber](https://github.com/GameMakerDiscord/Rubber) ⭐ 33 | 🐛 5 | 🌐 TypeScript | 📅 2021-02-20 - Compile GameMaker projects via the command line. Here's a [great guide](https://www.patreon.com/posts/how-to-build-36556955) on how to use it.
* [vim-GML](https://github.com/JafarDakhan/vim-gml) ⭐ 14 | 🐛 0 | 🌐 Vim Script | 📅 2022-10-04 - High quality Vim syntax highlighting for GameMaker.
* [GMLC](https://github.com/tinkerer-red/GMLC) ⭐ 9 | 🐛 57 | 🌐 Game Maker Language | 📅 2025-12-24 - Runtime compiler and interpreter to load, compile, and execute GML code at runtime.
* [Stitch for VSCode](https://marketplace.visualstudio.com/items?itemName=bscotch.bscotch-stitch-vscode) - Edit GameMaker projects in VSCode.
* [YYP Maker](https://sahaun.itch.io/yyp-maker) - Makes `.yyp` files for you.
* [GMSnip](https://manta-ray.itch.io/gmsnip) - Experimental tool to define unlimited code snippets in the IDE.
* [sfGML](https://yellowafterlife.itch.io/gamemaker-haxe) - Generate GML code from strongly-typed Haxe.
* [Win7 patcher for GM2024.11+](https://yellowafterlife.itch.io/gm2024-win7-patcher) - Makes games made in new GM versions run on Windows 7.
* [RerouteAudio](https://yellowafterlife.itch.io/gamemaker-reroute-audio) - Organizes audio files compiled games into subdirectories. 💸

## Debugging

* [rt-shell](https://github.com/daikon-games/rt-shell) ⭐ 92 | 🐛 2 | 🌐 Game Maker Language | 📅 2023-07-11 - Easy to use in-game shell. Create your own commands, command meta data, command suggestions, history, etc.
* [Crispy](https://github.com/bfrymire/crispy) ⭐ 42 | 🐛 7 | 🌐 Game Maker Language | 📅 2025-11-26 - Unit testing in GameMaker.
* [Snitch](https://github.com/JujuAdams/Snitch) ⭐ 36 | 🐛 3 | 🌐 Game Maker Language | 📅 2025-09-09 - Crash and logging system.
* [Gobo](https://github.com/Pizzaandy/Gobo/) ⭐ 28 | 🐛 4 | 🌐 C# | 📅 2025-11-21 - An opinionated code formatter for GML.
* [gms2-test](https://github.com/pmarincak/gms2-test) ⭐ 27 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-12-27 - Unit testing framework.
* [Olympus](https://github.com/bscotch/olympus#readme) ⭐ 20 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-05-13 - Testing Framework.
* [Lookout](https://github.com/glebtsereteli/Lookout) ⭐ 18 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-28 - Helpful debug overlay views.
* [Inspectron](https://github.com/shdwcat/Inspectron) ⭐ 16 | 🐛 1 | 🌐 Game Maker Language | 📅 2024-06-19 - A fluent API for easily creating GameMaker debug views.
* [Duck](https://github.com/imlazyeye/duck) ⭐ 14 | 🐛 0 | 🌐 Rust | 📅 2025-06-05 - A fast GML analyzer to enforce code styling and detect errors.
* [Meta](https://github.com/nommiin/meta) ⭐ 8 | 🐛 0 | 🌐 Game Maker Language | 📅 2020-08-15 - Runtime asset inspector.
* [DeerLog](https://mulfok.itch.io/gamemaker-deerlog) - Small log writer.
* [FPS Speedometer](https://dragonite.itch.io/fps-speedometer-for-gamemaker) - Pretty framerate display.
* [GMPulse](https://topherlicious.itch.io/gmpulse) - A runtime inspector and control panel. 💸

## Input Handling

* [Good Vibes](https://github.com/mrdaneeyul/good-vibes) ⭐ 24 | 🐛 0 | 🌐 Yacc | 📅 2022-11-24 - Device vibration.
* [InputCandy](https://github.com/LAGameStudio/InputCandy) ⭐ 18 | 🐛 6 | 🌐 Game Maker Language | 📅 2025-03-14 - Similar to Input as it acts as a wrapper for SDL, with actions and signalling, but also provides testing, on-screen diagnostics, and some other UI components related to peripherals, as well as pre-built end-user configuration menus that can be easily restyled.
* [Mouse Queue](https://github.com/YAL-GameMaker/window_mouse_queue) ⭐ 6 | 🐛 0 | 🌐 HTML | 📅 2024-07-14 - Tracks the Windows mouse pointer with high precision.
* [Input](https://github.com/JujuAdams/input) ⭐ 0 | 🐛 0 | 📅 2026-01-29 - No nonsense gamepad/keyboard library.
* [XeroInput](https://www.reddit.com/r/gamemaker/comments/icoh6m/xeroinput_gms23_input_handler/) - Another library to handle multiple inputs for a single action.
* [Native Cursors](https://yellowafterlife.itch.io/gamemaker-native-cursors) - System-level custom cursors. 💸
* [Native Mouselock](https://yellowafterlife.itch.io/gamemaker-native-mouselock) - System-level mouse locking. 💸
* [Raw Input](https://yellowafterlife.itch.io/gamemaker-raw-input) - Use multiple mice and keyboards. 💸

## User Interface

* [Scribble](https://github.com/JujuAdams/scribble) ⭐ 393 | 🐛 28 | 🌐 Game Maker Language | 📅 2026-01-29 - Efficient multi-effects text renderer.
* [Chatterbox](https://github.com/JujuAdams/chatterbox) ⭐ 166 | 🐛 8 | 🌐 Game Maker Language | 📅 2026-02-04 - Narrative scripting tool.
* [Crochet](https://github.com/FaultyFunctions/Crochet) ⭐ 98 | 🐛 9 | 🌐 JavaScript | 📅 2021-11-22 - An interactive dialogue editor for writers and programmers.
* [Textboxy](https://github.com/glitchroy/textboxy) ⭐ 65 | 🐛 9 | 🌐 Game Maker Language | 📅 2023-03-05 - Simple textboxes.
* [YUI](https://github.com/shdwcat/YUI) ⭐ 63 | 🐛 39 | 🌐 Game Maker Language | 📅 2026-01-06 - A UI system with live reloading, template system, data binding, and a drag and drop feature.
* [NotificationSystem](https://github.com/babaganosch/NotificationSystem) ⭐ 44 | 🐛 0 | 🌐 Yacc | 📅 2023-12-28 - Notifications in GameMaker.
* [Emu UI](https://github.com/DragoniteSpam/Emu) ⭐ 40 | 🐛 5 | 🌐 Game Maker Language | 📅 2025-12-29 - Common UI elements (text input, checkboxes, radio buttons, dialog boxes, etc).
* [LimeUI](https://github.com/Limekys/LimeUI) ⭐ 32 | 🐛 3 | 🌐 Game Maker Language | 📅 2025-09-29 - Flexpanel system for modern, touch-friendly interfaces.
* [GMUI-Framework](https://github.com/AlertStudios/GMUI-Framework) ⭐ 29 | 🐛 21 | 🌐 Game Maker Language | 📅 2021-07-20 - A pure GML solution to structure and control your menus, drawing parallels to .NET UI.
* [Guido](https://github.com/JujuAdams/Guido) ⚠️ Archived - Simple immediate mode GUI framework.
* [GMUI](https://github.com/erkan612/GMUI) ⭐ 18 | 🐛 1 | 🌐 Game Maker Language | 📅 2026-02-09 - Immediate mode GameMaker UI library, tons of UI components.
* [GMS2-UI-Library](https://github.com/nabilatsoulcade/GMS2-UI-Library) ⭐ 17 | 🐛 0 | 🌐 Yacc | 📅 2018-01-11 - A Library Full of useful scripts for implementing your UI designs in GameMaker.
* [SimpleUI](https://github.com/evolutionleo/SimpleUI) ⭐ 9 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-05-07 - Minimalistic UI framework.
* [zitk](https://github.com/TandyRum1024/zitk) ⭐ 6 | 🐛 0 | 🌐 Yacc | 📅 2022-06-26 - Another interesting, Dear ImGui-inspired GUI toolkit. In development, but worth keeping an eye on.
* [MajorGUI](https://github.com/erkan612/MajorGUI_GML) ⭐ 2 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-02 - Surface-based GUI that allows 100% control over UI styling and functionality.
* [Scripture](https://pixelatedpope.itch.io/scripture) - Another easy to use, highly compatible text renderer.
* [Easy And Fast Menu](https://pkgames.itch.io/easy-and-fast-menus-for-gms-23) - Simple implementation to have a menu up and running in seconds. Seems like a great fit if you're not looking for a bigger solution like GMUI.
* [Pause Menu](https://jasontomlee.itch.io/pause-menu-gamemaker-1-2) - Another smaller implementation but has a cool animation between menu options.
* [Magpie](https://dragonite.itch.io/magpie) - Generic Inventory System.
* [ImGuiGML](https://rousr.itch.io/imguigml) - DLL/GML wrapper of Dear ImGui.
* [GUI Framework](https://niris.itch.io/gui-framework) - GUI implementation from Niris Games.
* [Menu Tutorial](https://www.youtube.com/watch?v=1ITZOrI2qkA\&list=PLSFMekK0JFgx2vmcCnttxxhrNVTjUB8R1) - FriendlyCosmonaut. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Smart Clickable GUI](https://www.youtube.com/watch?v=RbBgE3cUShc) - Pixelated Pope. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [gooey](https://manta-ray.itch.io/gooey) - Sprite-based UI Library for GameMaker LTS.

## Localization

* [lexicon](https://github.com/tabularelf/lexicon) ⭐ 50 | 🐛 1 | 🌐 Game Maker Language | 📅 2025-12-22 - Another localization solution focused on simplifying implementation.
* [polyglot](https://github.com/daikon-games/polyglot) ⭐ 31 | 🐛 2 | 🌐 Game Maker Language | 📅 2024-02-03 - Localization library.
* [gm-i18n](https://github.com/CreativeHandOficial/gm-i18n) ⭐ 21 | 🐛 0 | 🌐 Yacc | 📅 2023-02-04 - Internationalization of texts simply and quickly, using JSON files.
* [Small Pentapop Localization Tool](https://github.com/AntonBergaker/small_pp_localization_tool) ⭐ 11 | 🐛 0 | 🌐 C# | 📅 2026-01-23 - Similar export tool to GMLocalize but exports to a csv.
* [GMLocalize](https://github.com/DragoniteSpam/GMLocalize2) ⭐ 5 | 🐛 0 | 🌐 C# | 📅 2022-07-05 - Not a full localization solution. Extracts text strings for localization from a GameMaker Studio 2 project and saves it to a JSON file.
* [gms2-mofile](https://github.com/pmarincak/gms2-mofile) ⭐ 3 | 🐛 0 | 🌐 C++ | 📅 2023-12-28 - Mofile reader used for localization.
* [cmnLoc](https://yellowafterlife.itch.io/gamemaker-cmn-loc) - Localization library with a text extractor, short syntax, and ICU/pluralization support. 💸
* [MythLoco](https://mythloco.co.uk) - A localization system with a web-based strings editor.
* [Krug's Localize System](https://krug-dev.itch.io/localize-system-for-gamemaker) - A localization system with real-time Google Sheets API synchronization.

## Physics

* [Loj Hadron Collider](https://github.com/Lojemiru/Loj-Hadron-Collider) ⭐ 40 | 🐛 2 | 🌐 Yacc | 📅 2022-10-28 - A robust, pixel-perfect collision engine.
* [GMVerlet-Integration](https://github.com/tabularelf/GMVerlet-Integration) ⭐ 11 | 🐛 0 | 🌐 Yacc | 📅 2021-06-10 - Verlet integration example used for visuals.
* [Inverse Kinematics Extension](https://github.com/tonystr/Inverse-Kinematics-Extension-for-Gamemaker) ⭐ 3 | 🐛 0 | 📅 2017-12-26 - A library for working with inverse kinematics.
* [On Slopes and Grids](https://forum.yoyogames.com/index.php?threads/on-slopes-and-grids-subpixel-perfect-topdown-movement-and-collision-line-without-objects.4073/) - A tutorial to implement 45° slopes.
* [GMS2 Platforming System](https://benal.itch.io/basic-modern-platforming-system) - GameMaker implementation by Ben Allen and an expansion on Shaun Spalding's original 1.4 platformer tutorial.
* [Verlet Integration Library](https://jamjamteam.itch.io/verlet-integration-gamemake-studio-2) - Verlet integration by Sarek Lambert.
* [Top-Down Movement & Collision](https://pixelatedpope.itch.io/tdmc/devlog/156556/converting-tdmc-to-use-tiles) - Robust object-based collision system from Pixelated Pope.
* [GMPhysX](https://bytecauldron.itch.io/gmphysx) - Adds NVIDIA PhysX to GameMaker for physics-based 2D/3D games. 💸

## Sprites

* [SpriteSource](https://github.com/bscotch/stitch/tree/develop/packages/sprite-source) ⭐ 149 | 🐛 26 | 🌐 TypeScript | 📅 2026-01-11 - Utilities for creating art asset pipelines.
* [PixelUpscaler](https://github.com/JujuAdams/Pixel-Art-Upscaling) ⭐ 36 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-12-31 - Pixel art upscaling shader for awkward resolutions for GameMaker.
* [Collage](https://github.com/tabularelf/Collage) ⭐ 29 | 🐛 7 | 🌐 Game Maker Language | 📅 2025-12-28 - Texture page builder and image manager. Mimics GameMaker's texture page packing while offering higher flexibility.
* [Disarm](https://github.com/NuxiiGit/disarm) ⭐ 24 | 🐛 3 | 🌐 Game Maker Language | 📅 2023-07-02 - A spriter skeletal animation at runtime.
* [AESnips](https://github.com/angelwire/AESnips) ⭐ 9 | 🐛 1 | 📅 2025-08-04 - A sprite playback system.
* [GM Animate](https://github.com/KormexGit/GM-Animate) ⭐ 8 | 🐛 3 | 🌐 Game Maker Language | 📅 2026-01-31 - Sprite animation manager.
* [conveyorbelt](https://github.com/imissmyfriends/conveyorbelt) ⭐ 6 | 🐛 2 | 🌐 JavaScript | 📅 2023-09-08 - Similar to ASESync. Export Aesprite files to GameMaker sprites.
* [phgen](https://github.com/squircledev/phgen) ⭐ 3 | 🐛 0 | 🌐 Game Maker Language | 📅 2021-11-16 - Placeholder asset generation.
* [ASESync](https://sahaun.itch.io/asesync) - Automatically syncs aesprite files in GameMaker.

## Audio

* [GMEXT-FMOD](https://github.com/YoYoGames/GMEXT-FMOD) ⭐ 72 | 🐛 1 | 🌐 HTML | 📅 2025-12-22 - Official support for FMOD in GameMaker.
* [Vinyl](https://github.com/JujuAdams/Vinyl) ⭐ 56 | 🐛 6 | 🌐 Game Maker Language | 📅 2026-01-28 - Live updating audio system.
* [Bard](https://github.com/gl326/bard-audio) ⭐ 40 | 🐛 2 | 🌐 Game Maker Language | 📅 2024-09-16 - An engine for desiging and implementing good audio in GameMaker. Updated to make use of the more recent GameMaker audio effects.
* [FML](https://github.com/Nikkilae/fml) ⭐ 7 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-03-08 - GameMaker bindings for the FMOD Studio API.
* [wavload](https://github.com/nkrapivin/wavload) ⭐ 7 | 🐛 0 | 🌐 NSIS | 📅 2020-10-05 - Demonstrates how to externally load .wav files.
* [audioExt](https://github.com/tabularelf/audioExt) ⭐ 5 | 🐛 1 | 🌐 Game Maker Language | 📅 2024-12-07 - Sound External Loader/Unloader Manager.
* [Phonix](https://github.com/Andre-404/Phonix/) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-06-18 - Compact audio system. Great for dynamic music!
* [LineAudio](https://github.com/WangleLine/LineAudio) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-11-08 - Audio helper functions.
* [ExternalAudio](https://github.com/NuxiiGit/ExternalAudio) ⭐ 1 | 🐛 0 | 📅 2019-02-27 - Load external .wav files at runtime.
* [Echo/Delay Effect](https://madwolf-studios.itch.io/audio-echodelay-effect-for-gamemaker-studio-2) - Optimized delay effect. 💸
* [SynthEngine](https://topherlicious.itch.io/synthengine) - A fully-featured musical synthesizer for GameMaker.
* [MusicTheoryLib](https://topherlicious.itch.io/musictheorylib) - Convenient music theory utilities for GameMaker.
* [WaveForm](https://topherlicious.itch.io/waveform) - Render audio wave forms from audio buffers in GameMaker.
* [WaveWrite](https://topherlicious.itch.io/wavewrite) - Read and write WAV files in GameMaker.
* [GMMidi](https://topherlicious.itch.io/gmmidi) - Read and write MIDI files in GameMaker.
* [EZAFX](https://topherlicious.itch.io/ezafx) - Instant preset audio effects for GameMaker.
* [GMSync](https://topherlicious.itch.io/gmsync) - Perfectly sync game elements to the rhythm of your music.
* [MicVol](https://topherlicious.itch.io/micvol) - Easily monitor microphone volume in real time in GameMaker. 💸

## Levels

* [GMRoomLoader](https://github.com/glebtsereteli/GMRoomLoader) ⭐ 105 | 🐛 1 | 🌐 Game Maker Language | 📅 2026-02-09 - Streamlined room loading at runtime. Great for reusable room prefabs and procedural generation.
* [LDtkParser](https://github.com/evolutionleo/LDtkParser) ⭐ 60 | 🐛 2 | 🌐 Game Maker Language | 📅 2025-08-14 - Advanced LDtk Importer.
* [Random Level Generator](https://github.com/GameMakerDiscord/random-level-gen-gms2) ⭐ 54 | 🐛 2 | 🌐 Game Maker Language | 📅 2018-03-03 - A random level generation example (similar to Nuclear Throne) using GameMaker.
* [Destructible Terrain](https://github.com/niksudan/gms2-destructible-terrain) ⭐ 31 | 🐛 2 | 🌐 Game Maker Language | 📅 2023-04-17 - An example of collidable, destructible terrain in GameMaker Studio using surfaces and grids.
* [Room Data Inspector](https://github.com/heygleeson/GM-RoomInspector) ⭐ 10 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-01-05 - Collects room data and stores it into a JSON for later use.
* [Random Dungeon Generator](https://github.com/BlaXun/Random-Dungeon-Generator-GMS-2.3) ⭐ 9 | 🐛 7 | 🌐 Yacc | 📅 2020-06-30 - Combines user-defined chambers to create a dungeon.
* [LDtk to GMS](https://shynif.itch.io/ldtk-to-gms) - LDtk Importer.
* [Wave Function Collapse](https://quadolorgames.itch.io/wfc-gml-demo) - Generates a random tile map but not production ready in its current state.
* [Cellular Automata Caves](https://alessiogamedev.itch.io/gms-cellular-automata-algorithm) - Generates huge caves in a few hundred milliseconds.

## Particles

* [Pulse](https://github.com/Delfos1/Pulse) ⭐ 23 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-14 - A library to create more complex particle emitters, systems and particles.
* [Burrn](https://github.com/FoxyOfJungle/Burrn) ⚠️ Archived - Built-in particle system that uses the particle asset built into the IDE.
* [Particles Wrapper](https://github.com/GamemakerCasts/particles) ⭐ 7 | 🐛 0 | 🌐 Yacc | 📅 2022-08-21 - A simplistic particle system wrapper that is designed to make creating particles fun and easy.
* [Particle Editor](https://gamemakercasts.itch.io/particle-editor) - Create particles with an easy UI and export into GML code.
* [Advanced Particles](https://limekys.itch.io/advanced-particle-system) - A particle implementation that comes with it's own delta timing methods.

## Lighting

* [Bulb](https://github.com/JujuAdams/Bulb) ⭐ 103 | 🐛 8 | 🌐 Game Maker Language | 📅 2025-11-17 - 2D lighting and shadows.
* [GameMaker Lighting Engine](https://github.com/bilouw/Gamemaker-Lighting-Engine) ⭐ 28 | 🐛 1 | 🌐 Game Maker Language | 📅 2019-02-15 - Tile-based Lighting Engine that projects shadows.
* [Lighting Systems](https://www.youtube.com/playlist?list=PLYVea5brHS8YHECGPoEp4_gWU-k6nWzUy) - Very fast dynamic 2D lighting implementation from GrizzliusMaximus using shadow casting. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Crystal](https://foxyofjungle.itch.io/crystal-2d-lighting-engine) - Complete and efficient 2D lighting & shadows solution. 💸

## Shaders

* [Outline Shader](https://github.com/Grisgram/gml-outline-shader-drawer) ⭐ 24 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-10-16 - Outline shader.
* [Bokeh Blur](https://github.com/XorDev/Bokeh/wiki) ⭐ 18 | 🐛 0 | 🌐 GLSL | 📅 2024-03-02 - Extension of the 1PassBlur which provides a different look. Similar to a real lens blur. Although it's much slower than 1Pass or Dual-Kawase.
* [Chameleon](https://github.com/Lojemiru/Chameleon) ⭐ 15 | 🐛 1 | 🌐 Yacc | 📅 2022-10-28 - Palette Swapper.
* [Xpanda](https://github.com/GameMakerDiscord/Xpanda) ⭐ 15 | 🐛 1 | 🌐 GLSL | 📅 2025-12-28 - Include code from external files in your shaders.
* [1PassBlur](https://github.com/XorDev/1PassBlur/wiki) ⭐ 13 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-01-15 - Blur Shader with adjustable radius.
* [Voronoi](https://github.com/XorDev/GMS-Voronoi-Pixels) ⭐ 13 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-05-18 - Sampled pixels on a Voronoi diagram.
* [Fire-Fun](https://github.com/XorDev/Fire-Fun/wiki) ⭐ 12 | 🐛 0 | 🌐 GLSL | 📅 2022-01-11 - Some fun magic fireballs.
* [Shadertoy to GameMaker](https://github.com/jfkn1ght/Shadertoy2GM) ⭐ 12 | 🐛 2 | 🌐 JavaScript | 📅 2025-07-10 - Convert shadertoy.com shaders to run in GameMaker (GLSL ES).
* [Dual-Kawase](https://github.com/XorDev/Dual-Kawase/wiki) ⭐ 11 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-02-20 - Blur Shader that limits radius but is very efficient.
* [TransFX](https://short-bread.itch.io/transfx) - Transition Library.
* [Post-Processing FX](https://foxyofjungle.itch.io/post-processing-fx) - 50+ high-quality, customizable effects. 💸
* [Lens Distortion FOV](https://foxyofjungle.itch.io/lens-distortion-fov-shader) - Useful FOV depth effect. 💸
* [Fast Blur Area](https://foxyofjungle.itch.io/foxey-blur-area) - Fast alpha blur shader effect in two lines of code. 💸
* [Transitions Pro](https://foxyofjungle.itch.io/foxey-transitions-pro) - 42 customizable transitions. 💸
* [Sketch Cartoon Shader](https://foxyofjungle.itch.io/sketch-cartoon-shader) - Turn your game visuals into a drawing/sketch style. 💸
* [2D Water Reflections](https://foxyofjungle.itch.io/water-reflective) - Customizable water object to easily display reflections. 💸
* [BJRTFX](https://zikbakguru.itch.io/bjrtfx) - Zik's CRT Utility Shader.
* [bktGlitch](https://odditica.itch.io/bktglitch) - Glitch shader.
* [H O R R I - F I](https://gizmo199.itch.io/horri-fi) - VHS Shader.
* [Depth Sorted Sillouettes](https://pixelatedpope.itch.io/depth-sorted-silhouette-example) - Example project to demonstrate shader-based depth sorting sillouettes. Tested on PC, Mac, HTML5, and Android.
* [GMShaders.com](https://gmshaders.com/) - Shader tutorials from Xor. Originally hosted at "xorshaders.com".
* [Xor's Halftone](https://xordev.itch.io/halftone) - A wonderful, versitile halftone shader. Lots of tweakable settings.
* [Jump Flooding](https://terohannula.itch.io/jump-flooding-algorithm) - Jump Flooding Algorithm for GameMaker made with shaders.
* [Shader Tutorials](https://www.youtube.com/watch?v=ch4BYqkL1w8\&list=PL0kTSdIvQNCNE-BDKOlYu628AalMmXy_P) - Gaming Reverends. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Shader Tutorials](https://www.youtube.com/watch?v=a4S7LXx6-sQ\&list=PL_hT--4HOvrdkihto8Xu7hhp1-5Gj8zsa) - DragoniteSpam. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)

## 3D

* [BBMOD](https://github.com/blueburn-cz/BBMOD) ⭐ 112 | 🐛 4 | 🌐 Game Maker Language | 📅 2026-02-08 - 3D Rendering Solution. Comes with several modules to import obj, 3D camera setup, integration with ColMesh, and more.
* [3D-2D](https://github.com/YoYoGames/3D-2D) ⭐ 48 | 🐛 2 | 🌐 Game Maker Language | 📅 2023-03-27 - Official tool to turn 3D models into 2D sprites.
* [dotobj](https://github.com/JujuAdams/dotobj) ⭐ 45 | 🐛 3 | 🌐 Game Maker Language | 📅 2025-10-12 - Lightweight .obj/.mtl 3D model loader written in native GML.
* [DmrVBM](https://github.com/Dreamer13sq/DmrVBM-blender-to-gms2) ⭐ 42 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-24 - Import/Export tools to load vertex buffer data out of Blender and into GMS.
* [Three Mice In a Trench Coat](https://github.com/XorDev/ThreeMiceInaTrenchcoat) ⭐ 10 | 🐛 0 | 🌐 Yacc | 📅 2021-06-25 - Source for a GameMaker 3D game.
* [Bronze Box](https://github.com/cicadian/Bronze-Box) ⭐ 4 | 🐛 0 | 🌐 Yacc | 📅 2022-07-23 - Example of how to build 3D world models from a 2D grid.
* [ColMesh](https://forum.yoyogames.com/index.php?threads/colmesh-3d-collisions-made-easy.82765/) - 3D Collision Library from TheSnidr.
* [BSP 4 GMS](https://cdlegasse.itch.io/ozarq-bsp-4-gms) - Import BSP files into GameMaker. Currently just a demo but worth keeping an eye on.
* [DopeFish Respawned](https://lemontoast-games.itch.io/dopefish-respawned) - Extensive WAD manager to load DOOM maps in GameMaker.
* [Blender to GameMaker](https://github.com/blender-to-gmstudio) - A collection of scripts to export and import Blender models to and from GameMaker.
* [Penguin](https://dragonite.itch.io/penguin) - 3D model conversion tool.
* [sPart](https://marketplace.yoyogames.com/assets/7299/spart-3d-particle-system) - 3D Particle System from TheSnidr.
* [Terrain Editor](https://dragonite.itch.io/terrain) - Terrain editor. Exports to gm models, obj, or vertex buffers.
* [Snowy Snow](https://dragonite.itch.io/snowy-snow) - 3D Snow Shader.
* [Collisions](https://dragonite.itch.io/collisions) - 3D collision system that works with native GML.
* [3D Fragment Point Lights](https://danieldavis.itch.io/ddg-point-light-shader-system) - 3D point lights using shaders. 💸
* [3D GameMaker Playlist](https://www.youtube.com/watch?v=ojfN--tdSNM\&list=PL_hT--4HOvrcML9uqHe4fwBVTm650Vy3V) - DragoniteSpam. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [3D Collisions Playlist](https://www.youtube.com/watch?v=o7kjtTEMpeU\&list=PL_hT--4HOvrf_VYo26LNl3zN5uwfuC3CC) - DragoniteSpam. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [3D Optimization Playlist](https://www.youtube.com/watch?v=knfAZbJJKNY\&list=PL_hT--4HOvrf_CJSA7fVU1tkjGVv5Sq2t) - DragoniteSpam. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [glTF parser](https://bitbucket.org/tijit/gltf-parser-for-gamemaker-lts/src/main/) - A model loader with support for animations.

## Sprite Stacking

* [Beginners Guide to Sprite Stacking](https://medium.com/@avsnoopy/beginners-guide-to-sprite-stacking-in-gamemaker-studio-2-and-magica-voxel-part-1-f7a1394569c0) - A primer on sprite stacking from Avis. Check out part 2 from dev\_dwarf as well.
* [Fauxton3D](https://gizmo199.itch.io/fauxton3d) - Sprite stacking engine.
* [Sprite Stacking Tutorials](https://www.youtube.com/watch?v=VIDN-nG3EOU\&list=PL3Kbpztq9qwT9MbW_k4yyJU__or1r8P2j) - Gizmo199. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)

## Networking

* [Warp](https://github.com/evolutionleo/Warp) ⭐ 141 | 🐛 0 | 🌐 TypeScript | 📅 2025-12-22 - A feature-rich framework for multiplayer games, written in GameMaker and Node.js.
* [Patchwire-GM](https://github.com/gm-core/patchwire-gm) ⭐ 34 | 🐛 0 | 🌐 Yacc | 📅 2020-09-13 - The network library from gm-core if you want to use this implementation without the entire gm-core suite.
* [MultiClient](https://github.com/tabularelf/MultiClient) ⭐ 29 | 🐛 1 | 🌐 Batchfile | 📅 2026-01-06 - Non-dll, multiple client launcher for network development.
* [HTTP GML](https://github.com/Sidorakh/http.gml) ⭐ 17 | 🐛 0 | 🌐 Game Maker Language | 📅 2026-02-09 - Recieve GET requests and upload files in GML.
* [GMNest](https://github.com/TimVN/GMNest) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2022-10-11 - Socket.IO extension for HTML5 games.
* [GM Networking](https://github.com/gmclan-org/gm_networking) ⭐ 2 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-08-06 - Very simple network code demonstration.
* [Boomers Networking](https://github.com/gmclan-org/gm_boomers_networking) ⭐ 2 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-08-06 - Network library which mimics pre-GM:Studio favorite networking extension 39dll using GM native functions.
* [EZ Networking](https://jasontomlee.itch.io/easy-gms-networking-platformer-build) - Host/client implementation with a chat feature.
* [GMHandshake](https://gist.github.com/nkrapivin/c73f5a962466a4ecb63187a009a300d8) - A Gist demonstrating a network handshake.
* [Multiplayer Networking Tutorial](https://www.youtube.com/watch?v=NbsXRuNijlo\&list=PLxaJReoxlrY_S4MrCYjzFCSrNX1TUX626) - Wizirdi. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Good GameMaker Rollback](https://springrollgames.itch.io/ggmr) - Rollback netcode library.
* [Rocket Networking Engine](https://marketplace.gamemaker.io/assets/11424/rocket-networking-engine) - Easy low-code multiplayer engine.

## Integrations

* [Steamworks.gml](https://github.com/YAL-GameMaker/steamworks.gml) ⭐ 91 | 🐛 2 | 🌐 C++ | 📅 2023-07-31 - Various expansions to Steamworks SDK support in GameMaker: Studio.
* [GMTwitch](https://github.com/GameMakerDiscord/GMTwitch) ⭐ 68 | 🐛 7 | 🌐 Game Maker Language | 📅 2022-01-03 - Twitch integration.
* [GMS2\_RPC](https://github.com/Mtax-Development/GMS2_RPC) ⭐ 11 | 🐛 0 | 🌐 C# | 📅 2025-10-07 - Another Discord integration.
* [GMHook](https://github.com/Kruger0/GMHook) ⭐ 11 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-04 - We really like Discord integration.
* [GOG.gml](https://github.com/GameMakerDiscord/GOG.gml) ⭐ 10 | 🐛 1 | 🌐 HTML | 📅 2023-07-30 - A native extension for GOG.com SDK support.
* [DHook](https://github.com/tabularelf/DHook) ⭐ 6 | 🐛 0 | 🌐 Yacc | 📅 2024-05-07 - Discord integration.
* [Parworks](https://github.com/nkrapivin/Parworks) ⭐ 3 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-06-30 - Additional functionality for the YYG Steamworks extension.
* [Github.gml](https://github.com/AlubJ/GitHub.gml) ⭐ 3 | 🐛 8 | 🌐 Game Maker Language | 📅 2026-01-20 - GitHub REST API
* [NekoPresence](https://marketplace.yoyogames.com/assets/9526/nekopresence) - Oops, all Discord integration.

## Camera

* [STANNcam](https://github.com/jack27121/STANNcam) ⭐ 43 | 🐛 15 | 🌐 Game Maker Language | 📅 2026-01-25 - Camera and resolution manager.
* [Pixel Perfect Smooth Camera](https://github.com/YAL-GameMaker/pixel-perfect-smooth-camera) ⭐ 38 | 🐛 0 | 🌐 Game Maker Language | 📅 2020-12-10 - An example of pixel-perfect yet smooth camera.
* [GameMaker Cameras: As Simple as Possible](https://www.youtube.com/watch?v=_g1LQ6aIJFk) - Pixelated Pope's guide on GameMaker's camera system. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Camera System Guide](https://maddestudiosgames.com/gms2-meet-the-camera-system/) - Getting started with cameras in GameMaker.
* [Dynamic Splitscreen](https://maddestudios.itch.io/gms2-project-dynamic-splitscreen) - Local multiplayer split screen implementation that merges the camera when players are close.
* [Camera All-In-One](https://jasontomlee.itch.io/allinone-camera) - Editor, screenshake, view-resizing, follow modes, screen effects, etc. 💸
* [REZOL](https://foxyofjungle.itch.io/rezol) - Complete resolution & screen manager (with split-screen support). 💸

## Sequences

* [Sequences Tutorial](https://www.youtube.com/watch?v=WO6gzhrx5b8) - Shaun Spalding. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Making Splash Screen Sequences](https://www.youtube.com/watch?v=hTh5UpFxx1E) - Mash Arcade. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [DuplicateSequence](https://github.com/KeeVeeGames/DuplicateSequence.gml) ⭐ 15 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-09-06 - Make a deep copy of sequence assets/structs for editing at runtime.

## State Machines

* [SnowState](https://github.com/sohomsahaun/SnowState) ⭐ 166 | 🐛 4 | 🌐 Game Maker Language | 📅 2025-06-29 - Robust finite state machine.
* [BehaviorTree](https://github.com/Gizmo199/BehaviorTree) ⭐ 11 | 🐛 0 | 🌐 Yacc | 📅 2023-12-18 - A simple behavior tree system.
* [Pinocchio](https://github.com/JujuAdams/Pinocchio) ⭐ 9 | 🐛 0 | 🌐 Yacc | 📅 2024-03-04 - State-based animation system.
* [FastSM](https://github.com/JulianDicken/FastSM) ⚠️ Archived - Lightweight alternative to SnowState.
* [FSM AI](https://github.com/gmclan-org/FSM-AI-module) ⭐ 5 | 🐛 0 | 🌐 Game Maker Language | 📅 2021-09-21 - Finite state machine for NPC AI.
* [wFSM](https://mors-games.itch.io/wfsm) - Another Easy-to-use Finite State Machine library.
* [True State](https://pixelatedpope.itch.io/truestate) - Feature-rich finite state machine to handle complex objects.

## Pathing

* [A-Star-Pathing](https://github.com/helloalbertdang/A-Star-Pathing) ⭐ 9 | 🐛 0 | 🌐 Game Maker Language | 📅 2021-02-06 - Another A\* pathfinding implementation.
* [Pathfinding in graph](https://github.com/gmclan-org/dijkstra-graph) ⭐ 6 | 🐛 1 | 🌐 Game Maker Language | 📅 2023-08-09 - Shortest pathfinding system in (weighted) graph, using Dijkstra algorithm.
* [Aquila](https://dragonite.itch.io/aquila) - A\* Pathfinding implementation.
* [Grid-based Pathfinding Scripts](https://proton-squid.itch.io/pathfinding) - Flexible pathfinding system with 3 different algorithms.
* [PathPlus](https://delfos1.itch.io/pathplus-for-gamemaker/devlog/1115089/pathplus-220-follower-and-spriter) - Enhance GameMaker Paths with CatmullRom and Bezier Interpolations.

## Useful Extras

* [OrbinautFramework](https://github.com/TrianglyRU/OrbinautFramework) ⭐ 114 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-12 - Accurate framework to make classic Sonic games.
* [Dracula Theme](https://github.com/dracula/gamemaker-studio) ⭐ 90 | 🐛 5 | 📅 2025-09-21 - A dark theme for the IDE.
* [CleanShapes](https://github.com/JujuAdams/Clean-Shapes) ⭐ 45 | 🐛 9 | 🌐 Game Maker Language | 📅 2026-02-03 - Antialiased primitives library for GameMaker.
* [Starfield Generator](https://github.com/PixelProphecy/gml_starfield_generator) ⭐ 31 | 🐛 1 | 🌐 Game Maker Language | 📅 2022-06-13 - A script to generate starfields in GameMaker's GML language.
* [Gruvbox Theme](https://github.com/heygleeson/Gruvbox-GMTheme) ⭐ 15 | 🐛 0 | 📅 2022-08-12 - A retro groove theme for the IDE.
* [Animated Flag](https://github.com/Grisgram/gml-animated-flag) ⭐ 13 | 🐛 0 | 🌐 Game Maker Language | 📅 2024-05-30 - Vertex-animated flag.
* [Danmaku Project](https://github.com/OmegaX1000/DanmakuProject) ⭐ 13 | 🐛 0 | 🌐 Yacc | 📅 2021-05-03 - Bullet hell engine.
* [GameMaker Repo Badges](https://github.com/matthiaszarzecki/MadeWithGameMakerStudioBadges) ⭐ 13 | 🐛 0 | 📅 2025-06-13 - Fancy badges to add to your README files.
* [Tome](https://github.com/chesrowe/Tome/) ⭐ 11 | 🐛 1 | 🌐 Game Maker Language | 📅 2026-02-03 - Automatically generate documentation sites from GameMaker projects.
* [Piano example](https://github.com/gmclan-org/piano_example) ⭐ 8 | 🐛 0 | 🌐 Game Maker Language | 📅 2023-02-17 - Example of playing intrument notes by changing pitch, using only one audio file.
* [Pause example](https://github.com/gmclan-org/pause_no_surface) ⭐ 4 | 🐛 0 | 🌐 Game Maker Language | 📅 2021-09-21 - Simple example of a pause screen without using surfaces.
* [Compatibility scripts](https://github.com/gmclan-org/compatibility-scripts) ⭐ 2 | 🐛 0 | 🌐 Game Maker Language | 📅 2022-04-11 - Scripts that are used by GM when importing GM:S 1.4 projects, taken directly from runtime files.
* [AssParser](https://github.com/DecadeDecaf/AssParser) ⭐ 0 | 🐛 0 | 🌐 Game Maker Language | 📅 2025-12-01 - Subtitle support for video playback.
* [Mouse Trail Effect](https://all-x.itch.io/gms2-mouse-trail-effect) - Shows how to trace a line with primitives to create a colorful trail.
* [GMLScripts.com](https://www.gmlscripts.com/script/index) - Dozens of helper scripts, organized similarly to the official documentation.
* [GM48 Resources](https://gm48.net/resources) - Free resources from the community to become better at GameMaker Studio, game development and game jams.
* [GameMaker Kitchen](https://www.gamemakerkitchen.com/) - Another great resource for open source libraries, assets, and snippets.
* [2.3 Syntax in Detail](https://yal.cc/gamemaker-2-3-syntax-in-details/) - A full guide of the syntax features/changes in GML from Yal.
* [GameMaker Garbage Collection](https://gist.github.com/DatZach/96a30d6ae4225f8ec152719e57aed26b) - How garbage collection works in GML.
* [GitHub Yacc to GML Fix](https://www.reddit.com/r/gamemaker/comments/n5m35l/a_simple_fix_for_github_incorrectly_detecting/) - Tell GitHub your repo is all GML, not Yacc.
* [GameMaker Discord Community GitHub](https://github.com/GameMakerDiscord) - Have you made a gamemaker tool you want to share? Consider submitting it to the official Discord's GitHub.
* [Source Control with Git & GameMaker](https://www.youtube.com/watch?v=UZG-P68xWio\&list=PLSFMekK0JFgzmyDxVxj5Cctafu5UX_vUC) - FriendlyCosmonaut. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Game Resolution & Aspect Ratio Management](https://www.youtube.com/watch?v=_g1LQ6aIJFk\&list=PLXkVsacazW2qvdnKNzgBLkUwlgi3FU-VO) - Pixelated Pope. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Setting up a Virtual Machine for GameMaker](https://www.youtube.com/watch?v=cK5k1_zN4eM) - MicahTheManiac. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Making Attacks Feel Good](https://www.youtube.com/watch?v=RWkMsD2WUz8) - Blobfish. ![YouTube](https://github.com/bytecauldron/awesome-gamemaker/raw/main/icons/youtube.png)
* [Build Automation, CI/CD](https://gist.github.com/shichen85/887d237cdc4338fa3f4e4749a14990db) - Tutorial on using GitHub Actions as a CI/CD pipeline to automate building games.
* [BROKVN](https://cowcat.itch.io/brokvn-engine) - A visual novel engine.
* [Ultimate Optimization Tier List](https://forum.gamemaker.io/index.php?threads/the-ultimate-gamemaker-optimization-tier-list.122141/) - Excellent forum thread on GameMaker optimization.

## Blogs

* [RefresherTowel](https://refreshertowelgames.wordpress.com/category/tutorial/) - Contains several posts on level generation.
* [Tony Str](https://tonystr.net/) - Some great articles on working with JSON, regular expressions *(regex)*, and drawing circles in GML.
* [Katsaii](https://www.katsaii.com/content/blog/posts.html) - Some articles on more advanced GML topics.
* [Meseta on Game Dev](https://meseta.dev/) - Seasoned GameMaker dev's thoughts on GameMaker concepts and libraries.
* [Thoughts On GameMaker](https://github.com/JujuAdams/ThoughtsOnGameMaker) ⭐ 51 | 🐛 0 | 📅 2025-11-28 - Not a traditional blog but has great info on different GML techniques.
* [YellowAfterlife](https://yal.cc/category/gm/) - Tutorials on intermediate/advanced topics.

## YouTube

* [Jordan Guillou](https://www.youtube.com/channel/UCBmOLRTaPrfOxnTqpCLrwdQ) - Hobbyist indie dev with a few GameMaker-related tutorials.
* [DragoniteSpam](https://www.youtube.com/c/DragoniteSpam) - Covers highly technical elements of GameMaker with a focus on 3D.
* [Shaun Spalding](https://www.youtube.com/c/ShaunSpalding) - Previous community manager at YoYo Games. Has a wide variety of beginner-friendly GameMaker tutorials and helpful updates on new GameMaker features.
* [FriendlyCosmonaut](https://www.youtube.com/c/FriendlyCosmonaut) - Great playlist on building a farming RPG in GameMaker with several other tutorials.
* [Pixelated Pope](https://www.youtube.com/c/PixelatedPope) - Guides on GameMaker resolution management, cameras, GUI, and more.
* [Xor](https://www.youtube.com/c/XorDev) - Tons of shader demonstrations with a focus on 3D.
* [GamingEngineer](https://www.youtube.com/c/GamingEngineer) - A GameMaker developer that has been in the community for many years. They have a wide variety videos showcasing what GameMaker is capable of, with a focus on 3D.
* [TheSnidr](https://www.youtube.com/c/TheSnidr) - A lot of awesome 3D showcases and tutorials for GameMaker.
* [Peyton Burnham](https://www.youtube.com/channel/UCfh2Q3TsvlxM1S2GvXQ4eeQ) - GameMaker tutorials for top-down shooters and RPGs.
* [Gaming Reverends](https://www.youtube.com/channel/UC7fkptPD1FHQyDc9Fnm9S_A) - If you want to learn foundational material regarding GameMaker shaders, the "Shaders for Hobby-Programmers" playlist is definitely worth checking out.
* [Let's Learn This Together](https://www.youtube.com/c/LetsLearnThisTogether) - Small indie dev company with a focus on providing GameMaker guides.
* [Matharoo](https://www.youtube.com/c/GameMakerStationMatharoo) - Tons of free GameMaker tutorials and news about GameMaker.
* [GravityShift Games](https://www.youtube.com/c/SlasherXGAMES/) - A couple of genre-specific GameMaker tutorials, integrating databases into GameMaker, and more.
* [Slyddar](https://www.youtube.com/c/Slyddar/) - A channel dedicated to both DnD and GML tutorials.
* [SamSpadeGameDev](https://www.youtube.com/@SamSpadeGameDev) - In-depth coding tutorials for the hobbyist game maker.
* [gentoo's iceberg Playlist](https://www.youtube.com/playlist?list=PLks6h7R6jAUGrofUAQB178r6K8h43Ml5-) - Series based on iceberg to display advanced programming ideas in GameMaker.

## Community

[![GameMaker Forums](https://img.shields.io/badge/Forums-6AA916?style=for-the-badge\&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAAAZlBMVEX%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2BrG8stAAAAIXRSTlMABg0OFBkfcn1%2Bf4CBgoOFhoeIiouWmNDa5ebp8PX2%2B%2F6o6Vq%2BAAAAY0lEQVR42k2OWQ6AIAwFn%2BIOioobrnD%2FS4o0EeanmQxNAdErRFTWtsFq6%2BiiZozz0CSnTjYBwo0RkF8DWDLf51Ni9K%2FYdq0Fy3KAfzk97M7goK1F%2F4rGH9Kk1OlboQtEDIrmC%2BU3CVxTr%2FRMAAAAAElFTkSuQmCC&\&logoColor=white)](https://forum.yoyogames.com/index.php)
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge\&logo=reddit\&logoColor=white)](https://www.reddit.com/r/gamemaker/)
[![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge\&logo=discord\&logoColor=white)](https://discord.gg/gamemaker)

## Special Thanks

JujuAdams, FaultyFunctions, Gleb Tsereteli, Shaun Spalding, DragoniteSpam, Nick Ver Voort, Pixelated Pope, Tony Strømsnæs, HeartBeast, Xor, Gaming Reverends, Matharoo, YellowAfterlife, Gizmo199, Avis, Josh Wilson, Lojemiru

## Footnotes

* If you need more general game development resources, check out [Awesome Gamedev](https://github.com/Calinou/awesome-gamedev) ⭐ 2,891 | 🐛 7 | 📅 2026-02-05 or [MagicTools](https://github.com/ellisonleao/magictools#readme) ⭐ 16,150 | 🐛 1 | 🌐 Markdown | 📅 2026-01-15.
* This is based on a list from [GameMaker Libraries](https://github.com/FaultyFunctions/GameMakerLibraries) ⭐ 3 | 🐛 0 | 📅 2021-08-09 and from Gleb Tsereteli with additional links/details.
* A majority of linked resources will only work with `GameMaker 2.3+` due to GML syntax changes. However, if you are working in GameMaker 1.4, most library creators would appreciate it if someone makes a backport of their project. 🙂

*GameMaker® is the property of YoYo Games™. This list is not affiliated with YoYo Games.*

## Contributing

Have something awesome to share? Check out the [Contributing Guidelines](https://github.com/bytecauldron/awesome-gamemaker/blob/main/CONTRIBUTING.md) ⭐ 443 | 🐛 1 | 📅 2026-01-08.

## GameMaker Keybindings

![Keybindings](https://github.com/bytecauldron/awesome-gamemaker/raw/main/images/keybindings.png)
