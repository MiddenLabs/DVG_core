# FROID Rules

_Derived from the MODE_ONE and MODE_TWO node bodies by `collate_three_rs.py`; the bodies are the source of truth (see AGENTS.md). Do not edit by hand._

## [GrammarRoot] — 02-00-00.00-00-00.00-00-00

- A01: [GrammarRoot] catalogs [Grammar_FS]

## [Grammar_FS] — 02-01-00.00-00-00.00-00-00

- A01: [Grammar_FS] catalogs [Ambient]
- A02: [Grammar_FS] catalogs [Stratum]

## [Ambient] — 02-01-00.01-00-00.00-00-00

- A01: [Ambient] defaults its frame to the present
- A02: [Ambient] defaults its mover to the self
- A03: [Ambient] defaults its well to the present place
- A04: [Ambient] is the one [Semarc] that can be known for certain
- A05: [Ambient] catalogs [Semarc]
- A06: [Ambient] catalogs [Supersession]
- A07: [Ambient] catalogs [Negation]
- A08: [Ambient] catalogs [Morphogenesis]
- A09: [Ambient] catalogs [Bracketing]
- A10: [Ambient] catalogs [TemporalReference]
- A11: [Ambient] catalogs [ModalReference]
- A12: [Ambient] catalogs [ReadingOrder]

## [Semarc] — 02-01-00.01-02-00.00-00-00

- A01: [Semarc] catalogs [Domain]
- A02: [Semarc] orders its [Domain] roles as [Frame] then [Mover] then [Well]
- A03: [Semarc] catalogs [Vector]
- A04: [Semarc] catalogs [Valence]
- A05: [Semarc] catalogs [Epistemic]
- A06: [Semarc] catalogs [Seme]
- A07: [Semarc] precedes each [Domain] with one [Vector]
- A08: [Semarc] is written at one [Stratum]
- A09: [Semarc] is revised by [Supersession]
- A10: [Semarc] writes each role as an [Epistemic] prefix then a [Vector] then a [Domain] then a [Valence] postfix

## [Domain] — 02-01-00.01-02-00.01-00-00

- A01: [Domain] catalogs [Frame]
- A02: [Domain] catalogs [Mover]
- A03: [Domain] catalogs [Well]
- A04: [Domain] catalogs [Descriptive]
- A05: [Domain] names a concept rather than a word
- A06: [Domain] takes its role from position
- A07: [Domain] may be a [Semarc]
- A08: an arc [Domain] may fill the [Frame], [Mover], [Well], or [Descriptive] slot
- A09: an operator on an arc [Domain] binds the whole [Semarc] as one [Seme]

## [Frame] — 02-01-00.01-02-00.01-01-00

- A01: [Frame] leads the [Semarc]
- A02: [Frame] carries the time context

## [Mover] — 02-01-00.01-02-00.01-02-00

- A01: [Mover] sits at the center of the [Semarc]
- A02: [Mover] is the origin the [Semarc] is reckoned from

## [Well] — 02-01-00.01-02-00.01-03-00

- A01: [Well] closes the [Semarc]
- A02: [Well] is where the [Mover] relation lands

## [Descriptive] — 02-01-00.01-02-00.01-04-00

- A01: [Descriptive] is written with a [CurlyBrace]
- A02: [Descriptive] narrows a [Domain] by overlap

## [Vector] — 02-01-00.01-02-00.02-00-00

- A01: [Vector] precedes a [Domain] in a [Semarc]
- A02: [Vector] catalogs [Self]
- A03: [Vector] catalogs [Toward]
- A04: [Vector] catalogs [Away]
- A05: [Vector] catalogs [Within]
- A06: [Vector] catalogs [Outside]
- A07: [Vector] catalogs [Inert]
- A08: [Vector] catalogs [NullVector]
- A09: [Vector] lets a motion value and a membership value hold at once toward one [Domain]

## [Self] — 02-01-00.01-02-00.02-01-00

- A01: [Self] marks the [Mover]
- A02: [Self] is written `~`
- A03: [Self] may also be written `«mv»`

## [Toward] — 02-01-00.01-02-00.02-02-00

- A01: [Toward] inverts to [Away]
- A02: [Toward] is written `\`
- A03: [Toward] may also be written `«to»`

## [Away] — 02-01-00.01-02-00.02-03-00

- A01: [Away] inverts to [Toward]
- A02: [Away] is written `/`
- A03: [Away] may also be written `«wa»`

## [Within] — 02-01-00.01-02-00.02-04-00

- A01: [Within] inverts to [Outside]
- A02: [Within] is written `@`
- A03: [Within] may also be written `«in»`

## [Outside] — 02-01-00.01-02-00.02-05-00

- A01: [Outside] inverts to [Within]
- A02: [Outside] is written `#`
- A03: [Outside] may also be written `«ot»`

## [Inert] — 02-01-00.01-02-00.02-06-00

- A01: [Inert] asserts non-interaction
- A02: [Inert] is written `.`
- A03: [Inert] may also be written `«un»`

## [NullVector] — 02-01-00.01-02-00.02-07-00

- A01: [NullVector] records a withheld relation
- A02: [NullVector] is written `_`
- A03: [NullVector] may also be written `«nl»`

## [Valence] — 02-01-00.01-02-00.03-00-00

- A01: [Valence] binds postfix to a [Seme]
- A02: [Valence] catalogs [Positive]
- A03: [Valence] catalogs [Negative]
- A04: [Valence] catalogs [Neutral]
- A05: [Valence] catalogs [Unsettled]
- A06: [Valence] catalogs [Undifferentiated]

## [Positive] — 02-01-00.01-02-00.03-01-00

- A01: [Positive] differentiates the [Undifferentiated] ring
- A02: [Positive] is written `°+`

## [Negative] — 02-01-00.01-02-00.03-02-00

- A01: [Negative] differentiates the [Undifferentiated] ring
- A02: [Negative] is written `°–`

## [Neutral] — 02-01-00.01-02-00.03-03-00

- A01: [Neutral] differentiates the [Undifferentiated] ring
- A02: [Neutral] is written `°0`

## [Unsettled] — 02-01-00.01-02-00.03-04-00

- A01: [Unsettled] differentiates the [Undifferentiated] ring
- A02: [Unsettled] is written `°%`

## [Undifferentiated] — 02-01-00.01-02-00.03-05-00

- A01: [Undifferentiated] is the ambient feeling ground
- A02: [Undifferentiated] is written `°`

## [Epistemic] — 02-01-00.01-02-00.04-00-00

- A01: [Epistemic] binds prefix to a [Seme]
- A02: [Epistemic] catalogs [Actual]
- A03: [Epistemic] catalogs [Interrogative]
- A04: [Epistemic] catalogs [Vouched]
- A05: [Epistemic] catalogs [Dubious]
- A06: [Epistemic] catalogs [Incredulous]
- A07: [Epistemic] catalogs [Distrust]

## [Actual] — 02-01-00.01-02-00.04-01-00

- A01: [Actual] cuts a slice from the [Ambient]
- A02: [Actual] is written `!`

## [Interrogative] — 02-01-00.01-02-00.04-02-00

- A01: [Interrogative] leaves actuality undetermined
- A02: [Interrogative] is written `?`

## [Vouched] — 02-01-00.01-02-00.04-03-00

- A01: [Vouched] reports the [Mover] trust in the record
- A02: [Vouched] is written `‼`

## [Dubious] — 02-01-00.01-02-00.04-04-00

- A01: [Dubious] reports the [Mover] doubt in the record
- A02: [Dubious] is written `⁉`

## [Incredulous] — 02-01-00.01-02-00.04-05-00

- A01: [Incredulous] reports the [Mover] disbelief in the record
- A02: [Incredulous] is written `⁇`

## [Distrust] — 02-01-00.01-02-00.04-06-00

- A01: [Distrust] reports the [Mover] distrust of the source
- A02: [Distrust] is written `⁈`

## [Seme] — 02-01-00.01-02-00.05-00-00

- A01: [Seme] bears an [Epistemic] prefix
- A02: [Seme] bears a [Valence] postfix
- A03: [Seme] may be a [Domain]
- A04: [Seme] may be a [Vector]
- A05: [Seme] may be an [Epistemic]
- A06: [Seme] may be a [Valence]
- A07: [Seme] nests operators without a fixed depth limit

## [Supersession] — 02-01-00.01-04-00.00-00-00

- A01: [Supersession] places the older [Semarc] on the lower line
- A02: [Supersession] keeps the operative [Semarc] on top
- A03: [Supersession] groups one event by indentation
- A04: [Supersession] bounds a timeline with a blank line that returns to the [Ambient]

## [Negation] — 02-01-00.01-06-00.00-00-00

- A01: [Negation] catalogs [Flip]
- A02: [Negation] catalogs [Demote]
- A03: [Negation] catalogs [Dissolve]

## [Flip] — 02-01-00.01-06-00.01-00-00

- A01: [Flip] inverts a [Vector]

## [Demote] — 02-01-00.01-06-00.02-00-00

- A01: [Demote] lowers a [Semarc] beneath its successor

## [Dissolve] — 02-01-00.01-06-00.03-00-00

- A01: [Dissolve] returns a [Seme] to the [Ambient]

## [Morphogenesis] — 02-01-00.01-07-00.00-00-00

- A01: [Morphogenesis] catalogs [Accretion]
- A02: [Morphogenesis] catalogs [Cleaving]

## [Accretion] — 02-01-00.01-07-00.01-00-00

- A01: [Accretion] mints a new [Domain]
- A02: [Accretion] mints a distinct [Domain] even from identical parts

## [Cleaving] — 02-01-00.01-07-00.02-00-00

- A01: [Cleaving] changes analytical resolution

## [Bracketing] — 02-01-00.01-08-00.00-00-00

- A01: [Bracketing] catalogs [SquareBracket]
- A02: [Bracketing] catalogs [CurlyBrace]
- A03: [Bracketing] catalogs [Paren]

## [SquareBracket] — 02-01-00.01-08-00.01-00-00

- A01: [SquareBracket] groups a [Domain]
- A02: [SquareBracket] is written `[ ]`

## [CurlyBrace] — 02-01-00.01-08-00.02-00-00

- A01: [CurlyBrace] describes a [Domain] without identifying it
- A02: [CurlyBrace] is written `{ }`

## [Paren] — 02-01-00.01-08-00.03-00-00

- A01: [Paren] groups an operator nest
- A02: [Paren] is written `( )`
- A03: [Paren] marks which level a nested operator operates at

## [TemporalReference] — 02-01-00.01-09-00.00-00-00

- A01: [TemporalReference] defaults time to the [Frame]
- A02: [TemporalReference] may place time as a [Domain]

## [ModalReference] — 02-01-00.01-0A-00.00-00-00

- A01: [ModalReference] places a condition in the [Frame]

## [ReadingOrder] — 02-01-00.01-0B-00.00-00-00

- A01: [ReadingOrder] reads the [Domain] first
- A02: [ReadingOrder] reads the [Vector] second
- A03: [ReadingOrder] reads the actuality [Epistemic] third
- A04: [ReadingOrder] reads the credence [Epistemic] fourth
- A05: [ReadingOrder] reads the [Valence] fifth

## [Stratum] — 02-01-00.02-00-00.00-00-00

- A01: [Stratum] catalogs [Stratum1]
- A02: [Stratum] catalogs [Stratum2]
- A03: [Stratum] catalogs [Stratum3]
- A04: [Stratum] catalogs [Collapse]

## [Stratum1] — 02-01-00.02-01-00.00-00-00

- A01: [Stratum1] writes every [Domain] and [Vector] and [Epistemic] in full
- A02: [Stratum1] leaves feeling undifferentiated

## [Stratum2] — 02-01-00.02-02-00.00-00-00

- A01: [Stratum2] drops ambient defaults by [Collapse]
- A02: [Stratum2] expands uniquely to [Stratum1]

## [Stratum3] — 02-01-00.02-03-00.00-00-00

- A01: [Stratum3] adds a differentiated [Valence]
- A02: [Stratum3] adds [Epistemic] credence

## [Collapse] — 02-01-00.02-04-00.00-00-00

- A01: [Collapse] drops the actual [Epistemic] default
- A02: [Collapse] drops the undifferentiated [Valence] default
- A03: [Collapse] drops the ambient [Frame] default
- A04: [Collapse] drops the [Self] [Mover] default
