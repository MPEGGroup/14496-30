# ISO/IEC 14496-30 — Working Draft

**Timed text and other visual overlays in ISO base media file format**

This repository holds the editors' **working draft** of ISO/IEC 14496-30, in a form that is easy
to read, review and contribute to.

> **This is not the official text.** It is a working draft maintained by the editors. It does not
> replace ISO/IEC 14496-30 as published by ISO/IEC, which is the only normative version.

**Read the draft:** https://mpeggroup.github.io/14496-30/

## Contributing

- Found an error, or want to propose a change? Please open an [issue](../../issues).
- Editorial fixes (typos, wording, broken references) can be sent as a pull request that changes
  the text in `bikeshed/`.
- Technical changes are discussed in the MPEG Systems group (ISO/IEC JTC 1/SC 29/WG 3) first.

## What is where

| | |
|---|---|
| `bikeshed/*.bs` | the text, one file per clause, in the order given by `bikeshed/manifest.txt` |
| `bikeshed/images/` | the figures |
| `bikeshed/header.bs` | the title, status and abstract of the draft |
| `specbuild.toml` | the settings of the build |
| `profiles.toml` | the build profile `github-wd` (HTML only, no ISO cover or boilerplate) |

The text is written in [Bikeshed](https://speced.github.io/bikeshed/). A paragraph is a plain
line of text; `<a href="#…">` is a cross-reference, and a formula is written between `\(` and `\)`.
Clause numbers are generated, not typed. The site on GitHub Pages is built from these files.

## Building the site

The page is built with the editors' build tool (Bikeshed underneath), which is not part of this
repository yet:

```
python compile.py --profiles-file profiles.toml --profile github-wd --output-dir <folder>
```

The result is published on the `gh-pages` branch. A pull request needs no build: the editors build
and publish after merging.

## Status

Working draft, converted from the consolidated text of the 2nd edition with Amendment 1
(m79110). Licence: *to be added by the maintainers before the first release.*
