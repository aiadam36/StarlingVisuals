# Upstream context

Starling Visuals was maintained in the Starling Android repository as
`packaging/shaderpacks/starling-visuals`. Its original description and feature summary are in
[`README.md`](https://github.com/horizon-rust/horizon/blob/main/README.md), and its development notes are in
[`roadmap/starling.md`](https://github.com/horizon-rust/horizon/blob/main/roadmap/starling.md).

The Android app embeds the pack by zipping that directory in
[`packaging/android/build_apk.py`](https://github.com/horizon-rust/horizon/blob/main/packaging/android/build_apk.py).
[`packaging/android/release_assets.py`](https://github.com/horizon-rust/horizon/blob/main/packaging/android/release_assets.py)
also creates a standalone `StarlingVisuals.zip` for a release. Those scripts belong to the Android app and are not
needed to use or edit this extracted pack.

The project's [MIT license](../LICENSE) applies to this extraction; the upstream pack directory did not contain a
separate license file. The clean-room specification and provenance record are included under [`cleanroom/`](cleanroom/).

## Pack history

These nine upstream commits directly changed the shaderpack. Their authors, dates and messages are preserved in this
repository's initial history; the file contents at every step were checked against the corresponding upstream tree.

- [`21237a0`](https://github.com/horizon-rust/horizon/commit/21237a070471cddcfb2fef0b1dc189b02ccef5fb) — initial pack
- [`d6a2f0f`](https://github.com/horizon-rust/horizon/commit/d6a2f0fe510769d33fd61b4d9fa503a248668df9) — shadows
- [`7f5ef14`](https://github.com/horizon-rust/horizon/commit/7f5ef144094b0379ab6e0d706189bdfd4cfd7b1b) — grounded shadows and softer edges
- [`ac1f33f`](https://github.com/horizon-rust/horizon/commit/ac1f33f1f63c1392a3b80cf374e416458cc98cad) — smoother shadow edges
- [`6234b37`](https://github.com/horizon-rust/horizon/commit/6234b3733b73fd042276e87739bd5e9840abd0da) — grass and crop shadow behavior
- [`338fa31`](https://github.com/horizon-rust/horizon/commit/338fa31eb68e061981d033225ea9ca31ccbaed41) — restore grass and leaf shadows
- [`af8f7cf`](https://github.com/horizon-rust/horizon/commit/af8f7cf49f4de2a1938846a59b0df1b37b034fec) — water waves and depth
- [`f3eafaa`](https://github.com/horizon-rust/horizon/commit/f3eafaae5ea907c3eca370043664d9f9c89cc88a) — haze, sun rays and bloom
- [`601558d`](https://github.com/horizon-rust/horizon/commit/601558da3197cec0aa8cb0e2f2ba5cc3a6e0d98a) — held-item light

Other related source commits cover the pack's app integration, release packaging, public description, and the
clean-room documentation. They remain in the original repository's history; this extraction keeps the pack's direct
code history and the relevant clean-room documents without importing unrelated Android or game changes.
