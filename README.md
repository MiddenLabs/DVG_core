# DVG

A grammar that reads cold.

Every node is a **FOLIO** — a directory holding a `.froid` manifest, an abstract
and a `.md` body, all sharing one NODE_ID. The body states what the node is and
the rules that bind it. Read it literally; the rules are mechanical, not advisory.

This namespace is **mechanics only**. It states true instructions and nothing
else — no rationale, no commentary, nothing to interpret. The *why* is not here.
It is either derivable from the rules, or recorded in ADR held privately.

The grammar's tree is `namespace/02-GrammarRoot`. It is a FROID namespace and
carries FROID's `00-SYSROOT` at the cut it was validated against:
[FROID_core](https://github.com/MiddenLabs/FROID_core) v1.0.0, the `FROID_core`
submodule (clone with `--recursive`); `namespace/00-SYSROOT` resolves into it.

Start at `namespace/02-GrammarRoot`. `[TAG]` cites another node;
`02-00-00.00-00-06.00-00-00.tagmap` at that root resolves the grammar's tags to
their NODE_IDs, and `00-SYSROOT`'s own tagmap resolves FROID's. In a node's
directory the abstract is `…-00.…-01.….md`, the manifest is the `.froid`, and
the body is `…-01.…-03.….md` (MODE_ONE).

`rules.md`, `restrictions.md`, `terms.md` and `reciprocals.md` under `namespace/`
are roll-ups collated from the grammar's bodies by tooling. Derived; the bodies
are the source.
