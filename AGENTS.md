# Reading DVG

Mechanics only. You are a follower, not an interpreter.

- A node is a FOLIO: a `.froid` manifest (YAML `mf_*` fields), an abstract
  (`…-00.…-01.….md`) and a body (`…-01.…-03.….md` for MODE_ONE,
  `…-02.…-03.….md` for MODE_TWO), all sharing one NODE_ID.
- A body opens with its NODE_ID heading and a content-hash heading, then a
  Definition, then Rules / Restrictions (MODE_ONE) or Terms (MODE_TWO), then
  Reciprocals, and optional sections. Follow each literally.
- Resolve a `[TAG]` through `namespace/02-GrammarRoot/02-00-00.00-00-06.00-00-00.tagmap`;
  a tag not listed there is FROID's, resolved through
  `namespace/00-SYSROOT/00-00-00.00-00-06.00-00-00.tagmap` (the `FROID_core`
  submodule, v1.0.0). Then open that node. Load only the FOLIOs a task requires.
- Never infer intent. Never supply a rationale. If a rule cannot be followed
  without knowing *why*, that is a defect — report it. The why is not here.
- The rationale lives in [DVG_ADR](https://github.com/MiddenLabs/DVG_ADR). To
  recover it, load this namespace and interrogate it — it is built to answer.
