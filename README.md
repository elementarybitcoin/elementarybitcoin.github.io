# Elementary Bitcoin

A free, community-driven mathematics textbook on Bitcoin.

**Read it: https://elementarybitcoin.org**

"Elementary" in the mathematician's sense: self-contained, not simple.
40 chapters and 4 appendices of numbered definitions, theorems, proofs,
and exercises — from the group axioms through secp256k1, Schnorr, SPV,
compact filters, Lightning, and Taproot, to the consensus cleanup and
the security budget. Every result is proved before it is used.

The five volumes are graded by epistemic status:

| Volume | Subject | Kind of truth |
|---|---|---|
| I | Mathematical Foundations (Ch 1–8) | proved mathematics |
| II | Protocol Architecture (Ch 9–17) | protocol fact, checkable against code and BIPs |
| III | Scaling and Verification (Ch 18–25) | protocol fact |
| IV | Forks and Futures (Ch 26–34) | the contested present, positions attributed and dated |
| V | The Path to a Sustainable Future (Ch 35–40) | disciplined speculation, labeled as such |

## Contributing

**An error found at any level is a contribution.** The claims of this
book are checkable: proofs can be re-derived, protocol facts checked
against running code and the cited BIPs, attributed positions verified
against their sources.

- **Errata:** [open an issue](../../issues) — say which chapter and
  section, what the text claims, and what is wrong with it. A reference
  (BIP, paper, source code) settles things fastest.
- **Fixes:** pull requests welcome. One issue per PR; reference the
  issue from the commit message.
- **New material:** the planned chapters most in need of authors are
  mempool and fee policy, wallet mathematics (BIP-32, descriptors,
  miniscript), mining pool economics, on-chain privacy, and the
  peer-to-peer network layer. Open an issue to coordinate before
  writing.

### House standards

Contributions are held to the book's voice (extracted from Volume I and
enforced book-wide):

- A claim is **proved**, **cited**, **computed and verified**, or
  explicitly marked as belief in a titled Remark. "Theorem" means proved
  or cited — nothing else wears the label.
- Contested or motive claims are attributed to their holders, never
  asserted in the book's voice. Perishable facts carry dates.
- Definitions define; product and proposal descriptions are Examples;
  practice notes are Remarks. Numbering is sequential per kind within
  each chapter.
- Calm "we"; no contractions, no exclamation marks, no second person
  outside exercises; colons over em-dashes.
- Figures that plot functions use paths computed from the equation,
  never drawn by hand. Diagrams use the house palette and Georgia
  labels (≥ 9px).
- Math is Unicode in `<span class="math">` / `<p class="math-block">`;
  placeholders that begin with a letter must be escaped
  (`&lt;sig&gt;`, or they vanish in HTML).

## Repository layout

- `index.html` — front matter and table of contents
- `chapters/NN-*.html` — the 40 chapters and appendices A–D
- `style.css` — single stylesheet for the whole book
- `llms.txt` — machine-readable summary

The site is static: open `index.html` in a browser, or serve the
directory with any static file server. Pushes to `main` deploy via
GitHub Pages.

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) —
free to share, correct, and build upon; derivatives stay open.

Written by Melvin Carvalho, with contributions from the community.
