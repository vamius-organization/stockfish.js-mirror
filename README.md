# Stockfish.js 19.0.1: an unmodified mirror

This repository is an **unmodified mirror** of [Stockfish.js](https://github.com/nmrugg/stockfish.js) by Nathan Rugg
and Chess.com, on [Stockfish](https://github.com/official-stockfish/Stockfish) by the Stockfish developers. It is kept
so that the Corresponding Source of the copy Chatorio gives out stays available, as section 6(d) of the GNU General
Public License, version 3, asks.

- **Upstream:** https://github.com/nmrugg/stockfish.js
- **The source of the build we give out:** tag
  [`v19.0.1`](https://github.com/vamius-organization/stockfish.js-mirror/tree/v19.0.1), commit
  `0d5dd7944f88c817c07a26bc4fb1905d5f9c46d6` (the same tag and commit as upstream). Nothing in it is changed.
- **The build:** `stockfish-19-lite-single.js` and `stockfish-19-lite-single.wasm`, made at that commit with
  `node build.js --single-threaded --lite -f` (the `build-single-lite` npm script; `build.js` expects Emscripten
  6.0.9), as published in the `stockfish` npm package, version 19.0.1. Chatorio serves those two files byte for byte,
  with SHA-256:
  - `stockfish-19-lite-single.js`: `ccb130d7ff29408531c47d859a49f91d59d4f482d05a53eb1a3231a4f624c91a`
  - `stockfish-19-lite-single.wasm`: `ee4f115bdb2d32cadf96cada104a05b5ec257d7ad6f57582190b49bc71f096de`
- **The network:** the build has the network `nn-61e7af4bb97d.nnue` built in (Stockfish 19's small "lite" network by
  Chris Bao, sscg13). It is not in the upstream repository; `make net` downloads it from Stockfish's network server,
  where every network is shared under **CC0**. A copy is kept here in [`nets/`](nets/), SHA-256
  `61e7af4bb97d51eeeb25d322916f86513b5cd3a827ce189c98c6e31946f99e5b`.
- **Licence:** GPL-3.0; the full text is [`Copying.txt`](Copying.txt), the same file as upstream's.

This branch holds only this note, the licence and the network. The source is on the tag. Report problems with
Stockfish or Stockfish.js upstream, not here.
