Here is a cleaned-up and well-formatted version of the content you shared, suitable for placing in a `README.md` file for your GitHub project:

````markdown
<div align="center">
  <img src="https://github.com/lllyasviel/Fooocus/assets/19834515/483fb86d-c9a2-4c20-997c-46dafc124f25" alt="Fooocus Banner">
</div>

# Fooocus

[👉 **Click Here to Install Fooocus** 👈](#download)

**Fooocus** is a powerful offline image generation software built on [Stable Diffusion XL (SDXL)](https://stability.ai/news/stable-diffusion-sdxl-10). It provides high-quality results with minimal manual tweaking, similar to services like Midjourney, but it's fully **offline**, **open-source**, and **free**.

> ⚠️ **Beware of fake websites claiming to be Fooocus.** The only official source is this GitHub page. We do **not** own any domains such as `fooocus.com`, `fooocus.ai`, etc.

---

## 🚦 Project Status

**Limited Long-Term Support (LTS)** – Only critical bug fixes. No new features or major updates are planned unless the community converges on a new standard image generation method.

For newer models like **Flux**, consider using:
- [WebUI Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge)
- [ComfyUI / SwarmUI](https://github.com/comfyanonymous/ComfyUI)
- [Community Forks](https://github.com/lllyasviel/Fooocus?tab=readme-ov-file#forks)

---

## ✨ Features

| Midjourney Feature | Fooocus Equivalent |
|--------------------|---------------------|
| Text-to-image with minimal prompt tuning | GPT-2 based prompt processor with improved sampling |
| V1–V4 Variations | Input → Upscale / Variation / Vary Subtle / Strong |
| U1–U4 Upscaling | Upscale to 1.5x or 2x |
| Inpaint / Pan | Built-in, custom inpainting models for better results |
| Image Prompt | Advanced algorithm for better understanding |
| --style | Advanced → Style |
| --no | Advanced → Negative Prompt |
| --ar | Advanced → Aspect Ratio |
| Prompt weights | `(word:1.5)`, similar to A1111 |
| Describe image | Input → Describe |
| ControlNet | Advanced image prompt control support |
| InsightFace | FaceSwap via image prompt tools |

> Learn more in [Advanced Features](https://github.com/lllyasviel/Fooocus/discussions/117)

---

## 📥 Download & Install

### 🔹 Windows (NVIDIA)

1. [Download Fooocus 2.5.0 (7z)](https://github.com/lllyasviel/Fooocus/releases/download/v2.5.0/Fooocus_win64_2-5-0.7z)
2. Extract the archive.
3. Run `run.bat`.
4. Wait for automatic model downloads (internet required once).

> 🛠 Requires at least **4GB VRAM (NVIDIA)** and **8GB RAM**

#### ✅ Optional Launchers:
- `run.bat` – Default
- `run_anime.bat` – Anime Preset
- `run_realistic.bat` – Realistic Preset

### 🔹 Google Colab

Run Fooocus in the cloud with one click:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lllyasviel/Fooocus/blob/main/fooocus_colab.ipynb)

Use presets like:

```bash
!python entry_with_update.py --share --always-high-vram --preset anime
````

### 🔹 Linux (Anaconda)

```bash
git clone https://github.com/lllyasviel/Fooocus.git
cd Fooocus
conda env create -f environment.yaml
conda activate fooocus
pip install -r requirements_versions.txt
python entry_with_update.py
```

Use `--preset anime` or `--preset realistic` as needed.

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

Follow standard install, then:

```bash
# Replace PyTorch with ROCm (Linux) or DirectML (Windows)
pip uninstall torch torchvision torchaudio
pip install torch-directml  # Windows
# OR
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.6  # Linux
```

Then run:

```bash
python entry_with_update.py --directml --preset anime
```

> ⚠️ AMD support is experimental.

---

## 🛠 Troubleshooting

* **Corrupted models** → Re-download model files
* **RuntimeError: CPUAllocator** → Enable virtual memory (swap) in Windows
* **Slow generation?** → Try NVIDIA driver v531 (older driver, better performance reported)

> See [Troubleshooting Guide](https://github.com/lllyasviel/Fooocus/blob/main/docs/troubleshoot.md) for more.

---

## 📸 Screenshots

<img src="https://github.com/lllyasviel/Fooocus/assets/19834515/938737a5-b105-4f19-b051-81356cb7c495" width="600">

---

<h2 style="color: red; margin-top: 15px; font-size: 28px;">Contact Information</h2>
<table style="width: 100%; margin-top: 15px; border-collapse: collapse;">
    <tr style="background-color: #64B5F6; color: #ffffff;">
        <th style="padding: 8px; border-bottom: 2px solid #000000;">Name</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">Email</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">LinkedIn</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">GitHub</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">Kaggle</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">LeetCode</th>
        <th style="padding: 8px; border-bottom: 2px solid #000000;">WhatsApp</th>
    </tr>
    <tr style="background-color: #FFFFFF; color: #000000;">
        <td style="padding: 8px;">Mustafa Shoukat</td>
        <td style="padding: 8px;">mustafashoukat.ai@gmail.com</td>
        <td style="padding: 8px;">
            <a href="https://www.linkedin.com/in/mustafashoukat/" target="_blank">
                <img src="https://img.shields.io/badge/LinkedIn-0e76a8.svg?style=for-the-badge&logo=LinkedIn&logoColor=white&style=flat-square" alt="LinkedIn Badge" style="border-radius: 50%; width: 80px;">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://github.com/Mustafa-Shoukat1" target="_blank">
                <img src="https://img.shields.io/badge/GitHub-171515.svg?style=for-the-badge&logo=GitHub&logoColor=white&style=flat-square" alt="GitHub Badge" style="border-radius: 50%; width: 80px;">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://www.kaggle.com/mustafashoukat" target="_blank">
                <img src="https://img.shields.io/badge/Kaggle-20beff.svg?style=for-the-badge&logo=Kaggle&logoColor=white&style=flat-square" alt="Kaggle Badge" style="border-radius: 50%; width: 80px;">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://leetcode.com/mustafashoukat" target="_blank">
                <img src="https://img.shields.io/badge/LeetCode-FFA116.svg?style=for-the-badge&logo=LeetCode&logoColor=white&style=flat-square" alt="LeetCode Badge" style="border-radius: 50%; width: 80px;">
            </a>
        </td>
        <td style="padding: 8px;">
            <a href="https://wa.me/923093609261" target="_blank">
                <img src="https://img.shields.io/badge/WhatsApp-25D366.svg?style=for-the-badge&logo=WhatsApp&logoColor=white&style=flat-square" alt="WhatsApp Badge" style="border-radius: 50%; width: 80px;">
            </a>
        </td>
    </tr>
</table>

