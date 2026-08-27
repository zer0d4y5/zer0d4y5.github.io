# zer0d4y5.github.io

Security research writeups by Elias Hasas ([@zer0d4y5](https://github.com/zer0d4y5)).

Published at <https://zer0d4y5.github.io/>.

## Contents

- **[CVE-2026-41992 — One array, two lives](posts/gzip-cve-2026-41992/)**
  GNU gzip: the first fix for the `.lzh`-after-`.Z` out-of-bounds read cleared the poisoned
  Huffman arrays in the branch that crashed, not in the function that reads them, leaving the
  sibling branch of the same `if` reading ~32 KB past the allocation. Fixed upstream in
  [`e7378c2d`](https://cgit.git.savannah.gnu.org/cgit/gzip.git/commit/?id=e7378c2d421be6a286922374425680bbe9ad8b7d)
  ("Problem and fix reported by Elias Hasas"); credited in gzip `THANKS` and in the CVE record.

## Building

Static HTML, no build step. `.nojekyll` is present so GitHub Pages serves the files as-is.
