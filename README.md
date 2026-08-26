# AI Agent Performance — published build

This repository holds one file: an encrypted build of a private dashboard.

`index.html` is AES-256-GCM ciphertext with a passphrase gate around it. The key is
derived in the browser with PBKDF2-SHA256 (310,000 iterations); the passphrase is
never transmitted. Without it there is nothing readable here.

Published by `tools/publish_site.py` from a private working copy. Source data,
tooling and exports are not in this repository.
