# 小兔播放器 / XiaoTu Player

SillyTavern third-party extension version of the 小兔播放器。

## Features

- Floating-player UI and existing visual design
- Playlist, play/pause, previous/next
- Loop / order / random playback modes
- Progress display and Media Session metadata
- Android/browser media controls when supported
- Background playback recovery based on the v55 implementation
- Nanjing map and existing non-music panels preserved

## Install

In SillyTavern: Extensions → Install Extension → paste this repository's Git URL.

This package is intended to be used as a third-party extension. It self-initializes after the page is ready.

## Important

This extension improves the player's lifecycle and keeps one persistent `<audio>` element instead of injecting the player through a Tavern Helper script. It cannot bypass an Android host/WebView that completely freezes or terminates background web execution.

## Source

Converted from `酒馆助手脚本-小兔播放器_v55_后台保活连续播放优化.json`.

## Favicon

This version replaces the SillyTavern page favicon with `assets/favicon.png` at runtime and guards it against the host page restoring the default favicon.


### v1.0.4
Fixed favicon loading for SillyTavern, which loads `index.js` as a classic script rather than an ES module. The extension now resolves `assets/favicon.png` from the actual extension script URL.
