# homebrew-tap

Homebrew tap for [@maheshj01](https://github.com/maheshj01)'s tools.

## Install

```bash
brew install maheshj01/tap/squish
```

Or try the latest `main` without a tagged release:

```bash
brew install --HEAD maheshj01/tap/squish
```

## Using squish

```bash
squish start              # begin watching ~/Movies/squish/clips
squish status             # settings + whether it's watching
squish config set CRF 20  # change a setting
squish clean              # empty clips AND compressed (asks y/N)
squish clean clips        # empty only the watched inputs
squish clean compressed   # empty only the compressed outputs
squish stop               # stop watching
```

Full docs: [maheshj01/squish](https://github.com/maheshj01/squish).

## Formulae

| Formula  | Description                                         | Source                                                  |
| -------- | --------------------------------------------------- | ------------------------------------------------------- |
| `squish` | Watch a folder and auto-compress videos with ffmpeg | [maheshj01/squish](https://github.com/maheshj01/squish) |

## Adding a new tool

1. Keep the tool's source in its own repo with a tagged release.
2. Add `Formula/<tool>.rb` here, with `url` pointing at that repo's release
   tarball (and `head` at its `main` for `--HEAD` installs).
3. Add a row to the table above.
