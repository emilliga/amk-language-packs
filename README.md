# AMK language packs

Public offline dictionary data for AMK. The application source remains private.
Download only the languages selected in AMK. Once installed, packs work offline.

Fourteen independent packs: English, Spanish, German, French, Italian, Hungarian,
Portuguese, Turkish, Chinese Simplified, Chinese Traditional, Japanese Kanji,
Japanese Hiragana, Japanese Katakana, and Hindi. Native-script candidates carry
source readings or derived Latin readings; coverage is finite and community data
can contain errors. This is not a continuous sentence conversion engine.

## Downloads and integrity

See [release v1](https://github.com/emilliga/amk-language-packs/releases/tag/language-packs-v1).
`language-packs.json` records exact URLs, compressed and expanded sizes, hashes,
licenses and source snapshots. Apps pin this catalog; packs are never executable
code. The gzip payload is an editable SQLite database, using `pack-schema.sql`.

## Sources and licenses

Wiktionary via Kaikki/Wiktextract, FrequencyWords/OpenSubtitles, CC-CEDICT/MDBG,
and JMdict/EDRDG are attributed in [licenses](licenses/). Dictionary data and
derived databases are CC BY-SA 4.0; upstream copyrights remain with their owners.
No private typing, personal vocabulary, signing material or application source
is included. Read [AMK's privacy information](https://emilliga.github.io/amk-language-packs/privacy.html).

## Updating the data

1. Preserve the published version and source hashes. Fetch updated upstream data
   from the source URLs in the catalog and record the new snapshot and hashes.
2. Prepare or edit the per-language SQLite database using the published schema.
   Native spelling, reading restrictions and original source-sense identifiers
   must be preserved. Do not join unrelated senses by English spelling.
3. Check SQLite integrity and inspect representative native and phonetic lookups.
   Compress with gzip (`mtime=0` for reproducibility), then compute SHA-256 for
   both the database and gzip and record their exact byte sizes.
4. Publish a new immutable version tag and catalog; never replace an existing
   file in a published release. The app catalog update follows app validation.
5. Review upstream updates regularly, including JMdict updates, and retain full
   attribution with every release. Source changes need native-speaker review.

The published SQLite files are the editable preferred form of these derived
data. Their source provenance is supplied for auditing and future refreshes.

## Product and support pages — 2 November 2026

GitHub Pages serves the product overview at index.html, setup/enrollment and
Not found troubleshooting at support.html, and updated SDK/download disclosures
at privacy.html. style.css and amk-icon.png are local assets; no tracking scripts,
forms, third-party fonts or dependencies were added. Keep release availability
honest and dated: Android closed test; iOS awaiting review at this checkpoint.
After a store status change, update those statements and the private app handover.
Do not publish tester addresses or claim that list membership proves enrollment.

## Link preview handover — 3 November 2026

Product, support and privacy pages now declare an absolute HTTPS Open Graph image, its actual 1254 × 1254 size, PNG type and alternative text, plus square social-card metadata and canonical URLs. The existing full-resolution brand asset is used without upscaling. The versioned image URL is `amk-icon.png?v=20261103`; change this version after future artwork updates. Previously sent messages may keep cached thumbnails. No messaging-app render has been verified.
