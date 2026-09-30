# KobeTools fork of DockDoor

Upstream: https://github.com/ejbills/DockDoor (branch `main`). Built from source with no auto-update. Re-check every row after each upstream sync.

## Fork changes

| Change | Where |
|---|---|
| Sparkle is never started; no background update check; "Check for Updates…" menu item removed | DockDoor/AppDelegate.swift |
| Upstream update feed and signing key removed | DockDoor/Info.plist |
| Release source build script (ad-hoc, no hardened runtime) | scripts/build-install-local.sh |

## Notes

- The SwiftFormat build phase runs `swift run swiftformat` from BuildTools/ (fetched as source from GitHub) and rewrites sources during builds.

## Syncing

Sync to upstream **release tags**, not the tip of `main`. From mactools run `scripts/audit-upstream.sh dockdoor`, merge only after review, then check every row above.
