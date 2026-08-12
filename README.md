# Fluent AOSP manifest

This manifest assembles the Fluent AOSP Android 17 source tree.

- Unmodified projects are pinned directly to Android Gitiles revisions.
- Modified projects are pinned to independent `Fluent-AOSP` repositories.
- Fluent project repositories begin with an exact tree snapshot from the recorded Android Gitiles commit and carry normal reviewable commits after that baseline.

Initialize and sync:

```bash
repo init -u https://github.com/Fluent-AOSP/android.git -b fluent-android17
repo sync --no-use-superproject
```

The manifest is revision-pinned. Branch names are provided for review and future updates; builds consume the recorded commit IDs.
