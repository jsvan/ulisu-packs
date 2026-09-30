# ulisu language packs

Offline dictionaries for the ulisu reading-to-flashcards app: one directory per language
(ISO 639-1 code), each with `latest.json` and versioned `v<N>/` folders holding `meta.json`,
`dict.tsv.gz` (root → English glosses, part of speech, frequency rank), `forms.tsv.gz`
(inflected form → root) and `rules.json.gz` (suffix rules). Built by `packs/` in the ulisu repo.

Served through jsDelivr from tagged releases, e.g.
`https://cdn.jsdelivr.net/gh/jsvan/ulisu-packs@v1/cs/v1/meta.json`.

## Sources and licence

Adapted from:

- **Wiktionary** via the [kaikki.org](https://kaikki.org/) extraction (wiktextract); text
  licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) (and GFDL).
  Wiktionary contributors: https://en.wiktionary.org/
- **FrequencyWords** by Hermit Dave (https://github.com/hermitdave/FrequencyWords), built from
  OpenSubtitles; content licensed CC BY-SA 4.0.
- Czech also uses glosses from the flashcards app's curated dictionary (built from the same
  Wiktionary data plus OPUS OpenSubtitles).

Each pack's `meta.json` lists its exact sources. Entries were filtered, normalized and
converted to the formats above. As adaptations of CC BY-SA material, the packs are licensed
**CC BY-SA 4.0** (see LICENSE).
