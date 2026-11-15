# LineageOS 16.0 for the Galaxy S5 Exynos (SM-G900H, k3gxx): releases

Unofficial LineageOS 16.0 (Android 9) builds for the Samsung Galaxy S5
SM-G900H (Exynos 5422).

- Downloads: see [Releases](https://github.com/stalex91/k3gxx-releases/releases).
- `lineage-16.0.json` is read by the built-in Updater
  (Settings → System → Updater) to offer new builds.
- Sources: [android_local_manifests_k3gxx](https://github.com/stalex91/android_local_manifests_k3gxx)
  (device tree, kernel and the changed LineageOS projects).
- Changelog: [CHANGELOG.md](CHANGELOG.md).

Builds are signed with the maintainer's own keys. Switching to them from a
build signed with other keys (official LineageOS, other ROMs, test-keys
builds) needs a clean install (Format Data in TWRP).

Each zip has a `.sha256sum` file next to it in the release:

```sh
sha256sum -c lineage-16.0-YYYYMMDD-UNOFFICIAL-k3gxx.zip.sha256sum
```
