# Liana — Spanish (es-ES)

Unofficial translation catalog for [Liana](https://github.com/wizardsardine/liana).
Not merged upstream.

`liana_es.lang`: **858 entries, 0 untranslated**. Base: master `9588ee3d` (2026-10-27).

Built from pythcoiner's [#2315](https://github.com/wizardsardine/liana/pull/2315),
realigned with the current `liana_en.lang` using `liana-i18n-toolbox sync` (151 entries
retranslated or added).

Terminology: billetera, frase mnemónica, dispositivo de firma, hardware wallet,
multifirma, clave caliente. Informal address (tú).

## Use

```sh
cd liana
cp /path/to/liana_es.lang liana-i18n/i18n/
cargo run -p liana-i18n-toolbox -- sync --verify
cargo run -p liana-i18n-toolbox -- check-ids
cargo build --release -p liana-gui && LANG=es_ES.UTF-8 ./target/release/liana-gui
```

## Verified

- `sync --verify` → catalogs are synced with liana_en.lang
- `check-ids` → passed (833 ids used)
- `cargo test -p liana-i18n` → 7 passed
- Builds into `liana-gui`, starts in Spanish with `LANG=es_ES.UTF-8`

## Limits

`es-ES` only · installer SVGs untranslated
([#2290](https://github.com/wizardsardine/liana/issues/2290)) · no UI width pass for a
sixth locale.

Produced with AI assistance, terminology reviewed by a human. Corrections welcome.
License: BSD-3-Clause, same as Liana.
