# Repository instructions

This is Lindoo's personal Orca plugin catalog. Keep it limited to plugins maintained in this repository.

Whenever a change modifies an existing `plugins/<name>/` directory, commit the plugin change first, then generate and commit its catalog release metadata:

```sh
ORCA_DIR=/path/to/orca node scripts/release-entry.mjs --write
```

Verify release metadata with:

```sh
ORCA_DIR=/path/to/orca node scripts/release-entry.mjs
```

Do not hand-author release hashes or release commit IDs.
