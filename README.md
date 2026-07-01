# Pet Society

A fan-made revival of Pet Society, the Playfish game that shut down in 2013. Rebuilt from scratch as a native app instead of the original Flash client.

The server is based on **[mascotsociety](https://github.com/DexterX12/mascotsociety)** by DexterX12, a from-scratch reimplementation of Playfish's backend. This project extends that emulator and builds a new client on top of it.

## What this actually is

The original game's Flash client can't run natively anymore. Rather than relying on a Flash emulator layer to keep it playable, this rebuilds the client from the ground up:

- original game assets, extracted and catalogued (~25,000 items) from archived swf files
- a custom asset format that keeps items editable instead of shipping flattened, pre-baked images
- a new renderer built on pixi.js, not Flash/Ruffle
- the server's network protocol and data model fully mapped, so the client talks to a real backend instead of faking state locally

## Status

Not playable yet. This is an active reconstruction project.

**Working:**
- asset extraction and packaging pipeline
- server protocol and data model, fully understood and documented internally
- a subset of the original server's actions: profile save/load, purchases, cooking, fishing, digging, quests

**Not working yet:**
- most of the original game's server actions (achievements, gifting, minigames, builder/DIY systems, and others)
- room and world rendering
- mobile build

## Platform

Android first, direct APK download, no Play Store initially. iOS later if the project gets there — that's a heavier lift (Mac hardware, Apple Developer account) and not a priority yet.

## Why this exists

Pet Society had no offline mode and no way to preserve it once Playfish shut the servers down. This is an attempt to bring it back in a form that doesn't depend on Adobe Flash still existing.

## Credit

- Server emulator: [mascotsociety](https://github.com/DexterX12/mascotsociety) by DexterX12
- Original game, assets, and IP belong to Playfish/EA. This is an unofficial fan project, not affiliated with either company.
