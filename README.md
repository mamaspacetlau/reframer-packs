# Reframer runtime packs

Optional GPU runtime packs downloaded by the Reframer engine (After Effects / Premiere Pro extension).
This repository holds **release assets only**; it contains no Reframer source code.

| Pack | File | Contents | Licence |
|---|---|---|---|
| DirectML (Windows, any DirectX 12 GPU) | `ort-directml-1.24.4.zip` | onnxruntime-directml 1.24.4 | MIT (Microsoft), third-party notices inside the zip |
| NVIDIA CUDA (Windows, NVIDIA GPU, driver 576.57 or later) | not hosted here | The engine installs it directly from the official PyPI wheels: onnxruntime-gpu (Microsoft) and NVIDIA's CUDA 12 and cuDNN 9 wheels (`nvidia-*-cu12`), checked against pinned SHA-256 hashes | onnxruntime-gpu: MIT (Microsoft). NVIDIA CUDA and cuDNN wheels: NVIDIA's licence terms, shipped with each wheel |

The engine pins each file's SHA-256 and size and refuses anything that doesn't match, so a replaced or corrupted asset is never loaded.

Downloads: see the [`packs` release](../../releases/tag/packs).
