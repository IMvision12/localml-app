# LocalML

> Browse the HuggingFace Hub. Download with a click. Run locally — detection, segmentation, classification, depth, OCR, SAM, VLMs, ASR, TTS, diffusion. **No cloud, no upload, your data never leaves your GPU.**

**Website**: https://www.localml.tech/

---

## What is this repo?

This is the **public home** of the LocalML desktop app — release artifacts, bug reports, feature requests. The application's source code is private; this repo is where:

- Installers are published (see [Releases](../../releases))
- Bugs and feature requests live (see [Issues](../../issues))
- Users can find the app and read its license

If you found this repo first, head over to **[localml.vercel.app](https://localml.vercel.app)** to download.

## What LocalML does

A desktop app (Windows, macOS, Linux) for running open-source ML models locally:

| Modality | Models |
|---|---|
| Vision | DETR, YOLOS, OWLv2, SegFormer, SAM 2/3, ViT, CLIP, SigLIP |
| VLM / Multimodal | Qwen-VL, LLaVA, Moondream, Florence-2, PaliGemma |
| Speech | Whisper, MMS-TTS, SpeechT5, Bark |
| Text | Llama, Mistral, Qwen, Phi, Gemma, DeepSeek |
| Diffusion | SD 1.5/XL, FLUX, SDXL-Turbo, Kandinsky |
| Embeddings | BGE, E5, all-MiniLM, BERT |
| Depth / OCR / DocQA | DPT, Depth Anything, TrOCR, LayoutLM |

200+ model families supported via the underlying transformers + diffusers runtime.

## Installing

1. Visit [localml.vercel.app](https://localml.vercel.app) and download the installer for your OS.
2. Run the installer.
3. **First launch only**: the app downloads a portable Python runtime (~30 MB) and installs PyTorch + transformers (~2–5 GB depending on CPU/GPU pick). Wait ~5 minutes.
4. Browse the Hub, install a model, run.

### Windows: SmartScreen warning

Because the app isn't yet code-signed, Windows shows a "Windows protected your PC" warning on first launch. Click **More info** → **Run anyway**. The warning won't reappear after the first install. Code signing is on the roadmap.

### macOS: Gatekeeper

macOS may refuse to open the app on first run. Right-click the app in `Applications` → **Open** → confirm. After the first run, Gatekeeper remembers and you can open it normally. Apple Developer ID signing is also on the roadmap.

### Linux

The `.AppImage` is portable — `chmod +x` it and double-click, or run from the terminal.

## Filing a bug

Open a [new issue](../../issues/new/choose) and pick the **Bug Report** template. Include:

- Your OS + version
- LocalML version (titlebar shows it)
- Steps to reproduce
- Any console output if you can grab it

## Filing a feature request

[New issue](../../issues/new/choose) → **Feature Request** template.

## License

The LocalML binary distribution is provided under the terms in [`LICENSE`](./LICENSE) — short version: free to use for any purpose, no warranties.

## Status

LocalML is in active development. Expect rough edges; please file issues when you find them.
