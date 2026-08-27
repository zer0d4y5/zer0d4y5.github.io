# zer0d4y5.github.io

Security research writeups by Elias Hasas ([@zer0d4y5](https://github.com/zer0d4y5)).

Published at <https://zer0d4y5.github.io/>.

## Contents

- **[A patch is a hypothesis](posts/gzip-lzh-walkthrough/)**
  Full walkthrough of checking someone else's fix: finding the aliased arrays by reading a
  header, proving the poison precondition before fuzzing, building a source-level oracle after
  AddressSanitizer stayed silent on a real out-of-bounds read, structure-aware generation, and
  shrinking a candidate from 41 bytes to 8. Every command and every output.

- **[One array, two lives](posts/gzip-cve-2026-41992/)** (CVE-2026-41992)
  GNU gzip: the first fix for the `.lzh`-after-`.Z` out-of-bounds read cleared the poisoned
  Huffman arrays in the branch that crashed, not in the function that reads them, leaving the
  sibling branch of the same `if` reading past the allocation. Fixed upstream in
  [`e7378c2d`](https://cgit.git.savannah.gnu.org/cgit/gzip.git/commit/?id=e7378c2d421be6a286922374425680bbe9ad8b7d)
  ("Problem and fix reported by Elias Hasas"); credited in gzip `THANKS` and in the CVE record.

## Building

Static HTML, no build step. `.nojekyll` is present so GitHub Pages serves the files as-is.
