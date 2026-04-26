# Ankimon Sprites

Pokemon sprites, sounds, and badge assets for the [Ankimon](https://github.com/h0tp-ftw/ankimon) Anki addon.

## Contents

| Folder | Files | Description |
|--------|-------|-------------|
| `front_default/` | ~3,300 | Front-facing Pokemon PNGs (including shiny + gender variants) |
| `front_default_gif/` | ~3,000 | Front-facing animated GIFs |
| `back_default/` | ~2,400 | Back-facing Pokemon PNGs |
| `back_default_gif/` | ~3,000 | Back-facing animated GIFs |
| `items/` | ~355 | Item sprites (pokeballs, potions, TMs, etc.) |
| `badges/` | ~68 | Achievement badge artwork |
| `sounds/` | ~1,000 | Pokemon cry sound effects (.ogg) |
| `missing_back/` | ~38 | Placeholder sprites for missing back views |

## Download

**For Ankimon users:** Sprites are downloaded automatically on first launch. You don't need to do anything.

**Direct download:**
- [GitHub Releases](https://github.com/h0tp-ftw/ankimon-sprites/releases/latest) (sprites.zip)
- [HuggingFace Mirror](https://huggingface.co/datasets/h0tp/ankimon) (sprites.zip via LFS)

## How it works

This repo is the single source of truth for all Ankimon sprite assets.

On every push to `main`, a GitHub Action:
1. Builds `sprites.zip` from the repo contents
2. Publishes it as a GitHub Release with SHA256 checksum
3. Pushes the ZIP to the HuggingFace mirror

Ankimon's download dialog fetches from these mirrors when a user first installs the addon.

## Contributing

To add or update sprites:
1. Fork this repo
2. Add/replace files in the appropriate folder
3. Open a PR

The ZIP and HuggingFace mirror update automatically on merge.

## License

All Pokemon-related imagery, names, and trademarks are the property of Nintendo, The Pokemon Company, and Game Freak. See [LICENSE](LICENSE) for full disclaimer.

Sprite assets sourced from [PokeAPI](https://github.com/PokeAPI/sprites) under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
