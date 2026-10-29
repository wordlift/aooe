# AOOE vocabulary

The `aooe:` vocabulary of **AOOE — Agent-Oriented Ontology Engineering**, the
WordLift methodology for building knowledge graphs that agents can act on.

- Namespace: `https://w3id.org/aooe#` (hash namespace; every term resolves to
  the one vocabulary document)
- Serialisations: [`aooe.ttl`](aooe.ttl) (source of truth), [`aooe.jsonld`](aooe.jsonld), [`aooe.owl`](aooe.owl)
- Documentation: <https://wordlift.github.io/aooe/>

Two groups of terms:

1. **Import-manifest terms** — how a package pins the vocabularies it reuses
   (`aooe:importedVocabulary`, `aooe:pinnedVersion`, `aooe:reuseMode`,
   `aooe:termsReused`, `aooe:servesACQ`, `aooe:governanceNote`) and relates its
   Behavioral Concept Specifications (`aooe:governs`, `aooe:refines`).
2. **Adoption levels** (methodology v0.7) — `Legend ⊂ Map ⊂ Rulebook`, cumulative:
   `aooe:AdoptionLevel`, `aooe:includesLevel`, `aooe:providesLevel` (what a
   package ships), `aooe:adoptsLevel` and `aooe:AdoptionRecord` (what a consumer
   takes, per use case). Only Rulebook-governed data lets an agent act.

This repository publishes the vocabulary only. The methodology, its gate
tooling and the client template are maintained separately by WordLift; this
file is released with each methodology version (`owl:versionInfo`).

## Licence

The vocabulary files in this repository (`aooe.ttl`, `aooe.jsonld`, `aooe.owl` and
the documentation page) are released under
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/),
stated on the ontology header as `dct:license`. Attribute to WordLift and link
to `https://w3id.org/aooe#`. The AOOE methodology, its gate tooling and the
client template are maintained separately and are not covered by this licence.

Maintainer: WordLift — <https://wordlift.io>
