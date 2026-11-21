# Agent instructions

This repository contains Starling Visuals, a GLSL shaderpack in the Iris/OptiFine pack format.

- Before changing shaders, read [the format specification](docs/cleanroom/shader-packs-spec.md) and [the provenance log](docs/cleanroom/provenance-log.md).
- Build from the documented pack format and the shader language specifications. Do not use shader-loader or renderer implementation source (including Iris, OptiFine, Oculus, Canvas, Sodium, or similar projects) as a model or source for code.
- Keep shared shader logic in `shaders/lib/` and stage-specific logic in the corresponding files under `shaders/`. Preserve documented pack interface names and explain any compatibility changes in the docs.
- Preserve project attribution and license notices. The pack had no separate license file upstream; this extraction includes the project's MIT license in `LICENSE`.
- When changing the provenance of the format specification, update `docs/cleanroom/provenance-log.md` in the same commit.
