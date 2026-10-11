# TRACE

Tail Reconstruction with Axial Context and Edge Supervision for road crack segmentation.

## Download the implementation

**[Download TRACE_Code_20261011.zip](TRACE_Code_20261011.zip)**

Extract the archive and open `TRACE/README.md` for environment requirements, data layout, dataset-specific configurations, and training/inference/evaluation commands. This repository currently distributes the implementation as a ZIP archive; the files are inside the archive.

SHA-256:

```text
990d4ac2be1eceb87633f7ac9003a0f0313011544fddcdecc1f94bbd3645bc47
```

## Included

- Model and retained MixerCSeg encoder source code.
- Gated cross-scale recovery, post-fusion axial context, and training-only supervision.
- Training, inference, dataset loading, and evaluation entry points.
- Filename-level split manifest and topology-evaluation helper.
- Bundled dependency source and third-party license notices.

The implementation retains its historical SCTR Python API names; the manuscript name is TRACE. Raw datasets, checkpoints, and private experiment outputs are not included.

## Verification scope

Packaging checks passed for 48 Python files, source-hash preservation, and an isolated decoder CPU forward/backward/evaluation smoke test. Full CUDA installation, end-to-end training, original-checkpoint compatibility, and reproduction of numerical manuscript results have not been revalidated for this release. See `TRACE/RELEASE_CHECKLIST.md` inside the archive.

The package README records the archived evaluation and checkpoint-selection protocol. The manuscript is in preparation for submission; no journal acceptance or publication is claimed.

## Attribution and licenses

This work builds on [MixerCSeg](https://github.com/spiderforest/MixerCSeg), with bundled [VMamba](https://github.com/MzeroMiko/VMamba) and Mamba-derived dependency code. Existing copyright notices are retained. The archive contains the original root license and separate third-party license texts; consult `TRACE/THIRD_PARTY_NOTICES.md` before reuse.
