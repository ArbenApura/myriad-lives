# Myriad Lives

An open-source, single-player, top-down action RPG set in a xianxia world of cultivators, sects and immortals.

- Pixel art and music made entirely by code: characters are code-defined models rendered to pixels, and the music comes from simulated instruments.
- A vast world at real scale that lives on its own, with time that runs like real time until you cultivate it away in seclusion.
- Complete freedom with real consequences: any path, anything can be destroyed, and the world remembers what you did.
- Many lives: death is permanent, and your next life can find your grave, your heirs and your legend.
- People who think, remember and talk.

## Status

Early development. Nothing is playable yet: the repository holds the workspace layout while the art and sound tests are built.

## Building

Rust is pinned in `rust-toolchain.toml`.

```
cargo build
cargo test --workspace
```

Targets: Windows and Linux. Saves, settings and logs are kept outside the repository, in `%LOCALAPPDATA%\myriad-lives` on Windows and the XDG data and config folders on Linux.

## Crates

| Crate | Purpose |
|---|---|
| `engine-core` | Shared engine foundations |
| `engine-render` | Indexed sprites, palette lookup, CPU and GPU rendering |
| `engine-audio` | Instrument synthesis, scores and mixing |
| `engine-ui` | Pixel font, text and widgets |
| `game-sim` | The deterministic simulation core |
| `game-worldgen` | Seeded world generation |
| `game-content` | Game content as RON data and its validator |
| `client` | The game |
| `tools` | Contact sheets, catalogue sheets and audio reports |

## Licence

Code, art, music and sound are dual-licensed under either of

- MIT licence ([LICENSE-MIT](LICENSE-MIT))
- Apache Licence, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE))

at your option. Third-party notices are in [THIRD-PARTY.md](THIRD-PARTY.md).

Unless you state otherwise, any contribution you submit for inclusion in this project is dual-licensed as above, without any additional terms or conditions.
