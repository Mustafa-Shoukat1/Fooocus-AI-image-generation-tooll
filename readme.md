<div align="center">
  <img src="https://github.com/lllyasviel/Fooocus/assets/19834515/483fb86d-c9a2-4c20-997c-46dafc124f25" alt="Fooocus Banner">
</div>

# Fooocus by Codagentic

[👉 **Click Here to Install Fooocus** 👈](#download)

**Fooocus** is a powerful offline image generation software based on [Stable Diffusion XL (SDXL)](https://stability.ai/news/stable-diffusion-sdxl-10), enhanced and maintained by **Mustafa Shoukat** at **Codagentic**. This version delivers Midjourney-like quality with full **offline**, **open-source**, and **free** capabilities.

> ⚠️ **Beware of fake websites claiming to be Fooocus.** The only official source is this GitHub page. We do **not** own domains such as `fooocus.com`, `fooocus.ai`, etc.

---

## 🚦 Project Status

**Limited Long-Term Support (LTS)** – Only critical bug fixes. No new features or major updates unless a community consensus emerges around new generation standards.

For newer models like **Flux**, try:
- [WebUI Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge)
- [ComfyUI / SwarmUI](https://github.com/comfyanonymous/ComfyUI)
- [Community Forks](https://github.com/lllyasviel/Fooocus?tab=readme-ov-file#forks)

---

## ✨ Features

| Midjourney Feature | Fooocus Equivalent |
|--------------------|---------------------|
| Text-to-image with minimal prompt tuning | GPT-2 based prompt processor |
| V1–V4 Variations | Upscale / Variation / Vary Subtle / Strong |
| U1–U4 Upscaling | Upscale to 1.5x or 2x |
| Inpaint / Pan | Built-in inpainting models |
| Image Prompt | Enhanced algorithmic support |
| --style | Style configuration in Advanced |
| --no | Negative prompts |
| --ar | Aspect ratio setting |
| Prompt weights | `(word:1.5)` format |
| Describe image | Use Describe tool |
| ControlNet | Advanced image prompt control |
| InsightFace | FaceSwap with tools |

More in [Advanced Features](https://github.com/lllyasviel/Fooocus/discussions/117)

---

## 📥 Download & Install

### 🔹 Windows (NVIDIA)

1. [Download Fooocus 2.5.0 (7z)](https://github.com/lllyasviel/Fooocus/releases/download/v2.5.0/Fooocus_win64_2-5-0.7z)
2. Extract the archive.
3. Run `run.bat`.
4. Wait for model downloads.

> 🛠 Requires **4GB VRAM (NVIDIA)** and **8GB RAM**

#### Optional Presets:
- `run.bat` – Default
- `run_anime.bat` – Anime
- `run_realistic.bat` – Realistic

### 🔹 Google Colab

Run in the cloud:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lllyasviel/Fooocus/blob/main/fooocus_colab.ipynb)

Example:

```bash
!python entry_with_update.py --share --always-high-vram --preset anime
```

### 🔹 Linux (Anaconda)

```bash
git clone https://github.com/lllyasviel/Fooocus.git
cd Fooocus
conda env create -f environment.yaml
conda activate fooocus
pip install -r requirements_versions.txt
python entry_with_update.py
```

### 🔹 Linux (Python venv)

```bash
git clone https://github.com/lllyasviel/Fooocus.git
cd Fooocus
python3 -m venv fooocus_env
source fooocus_env/bin/activate
pip install -r requirements_versions.txt
python entry_with_update.py
```

### 🔹 AMD GPU (Windows/Linux)

```bash
pip uninstall torch torchvision torchaudio
pip install torch-directml  # Windows
# OR
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.6  # Linux

python entry_with_update.py --directml --preset anime
```

> ⚠️ AMD support is experimental.

---

## 🛠 Troubleshooting

- **Corrupted models** → Re-download model files
- **RuntimeError: CPUAllocator** → Enable swap memory
- **Slow generation?** → Try NVIDIA driver v531

More: [Troubleshooting Guide](https://github.com/lllyasviel/Fooocus/blob/main/docs/troubleshoot.md)

---

## 📸 Screenshots

<img src="https://github.com/lllyasviel/Fooocus/assets/19834515/938737a5-b105-4f19-b051-81356cb7c495" width="600">

---

## 👨‍💻 Maintained By

### Mustafa Shoukat | Founder at Codagentic

<table style="width: 100%; margin-top: 15px; border-collapse: collapse;">
    <tr style="background-color: #64B5F6; color: #ffffff;">
        <th style="padding: 8px;">Name</th>
        <th style="padding: 8px;">Email</th>
        <th style="padding: 8px;">LinkedIn</th>
        <th style="padding: 8px;">GitHub</th>
        <th style="padding: 8px;">Kaggle</th>
        <th style="padding: 8px;">LeetCode</th>
        <th style="padding: 8px;">WhatsApp</th>
    </tr>
    <tr style="background-color: #FFFFFF; color: #000000;">
        <td style="padding: 8px;">Mustafa Shoukat</td>
        <td style="padding: 8px;">mustafashoukat.ai@gmail.com</td>
        <td style="padding: 8px;">
            <a href="https://www.linkedin.com/in/mustafashoukat/" target="_blank">
                <img src="https://img.shields.io/badge/LinkedIn-0e76a8.svg?style=for-the-badge&logo=LinkedIn&logoColor=white" alt="LinkedIn Badge">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://github.com/Mustafa-Shoukat1" target="_blank">
                <img src="https://img.shields.io/badge/GitHub-171515.svg?style=for-the-badge&logo=GitHub&logoColor=white" alt="GitHub Badge">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://www.kaggle.com/mustafashoukat" target="_blank">
                <img src="https://img.shields.io/badge/Kaggle-20beff.svg?style=for-the-badge&logo=Kaggle&logoColor=white" alt="Kaggle Badge">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://leetcode.com/mustafashoukat" target="_blank">
                <img src="https://img.shields.io/badge/LeetCode-FFA116.svg?style=for-the-badge&logo=LeetCode&logoColor=white" alt="LeetCode Badge">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://wa.me/923093609261" target="_blank">
                <img src="https://img.shields.io/badge/WhatsApp-25D366.svg?style=for-the-badge&logo=WhatsApp&logoColor=white" alt="WhatsApp Badge">
            </a>
        </td>
    </tr>
</table>
