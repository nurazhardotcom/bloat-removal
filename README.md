# bloat-removal

Dead-code elimination loop, regression-gated. Local only; see the
generalized harness spec in `nurazhardotcom/mcf-bot` `ARCHITECTURE.md`.

- `bin/bloat-removal scan [dir]` reports Lisp definitions with no
  references. Proposals only: delete only after the host repo's full
  regression selftest passes; a red gate discards the candidate.
- `bin/bloat-removal selftest` gates changes to this tool.
- `harness.edn` is the plug-in manifest.
