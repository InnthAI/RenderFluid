# RenderFluid

**RenderFluid** is a modular, secure, and easy-to-use AI generation pipeline for ComfyUI—designed for real-world deployment in creative, commercial, and regulated environments. It brings together curated models, SFW-first safety layers, consent enforcement (via NILE), and optimized batch workflows for illustration, photo realism, and upscaling.

With RenderFluid, you can generate high-quality AI content without writing a line of code, switching models mid-run, or worrying about unsafe outputs. Whether you're producing art, media, marketing, or internal tools, RenderFluid gives you speed, control, and auditability—all with plug-and-play simplicity.

## 🛠️ Getting Started with RenderFluid

Before using RenderFluid, you'll need to set up **ComfyUI**, install the required models, and prepare your environment. This section will walk you through the initial steps and point you to the official setup instructions for anything ComfyUI-specific.

---

### ✅ 1. Install ComfyUI

We recommend using the **ComfyUI Windows Portable Installer** for the easiest setup. It includes all dependencies and a built-in Python environment.

Follow the official ComfyUI installation instructions here:  
https://github.com/comfyanonymous/ComfyUI

This guide will show you how to:
- Download and run the installer
- Launch the interface in your browser
- Install custom nodes and workflows

> RenderFluid is installed like any other custom node—by cloning or downloading it into your `ComfyUI/custom_nodes/` folder.

---

### 📦 2. Download the Required Models

To use the full RenderFluid workflows, you’ll need to download at least one of the following **checkpoints** (base AI models):

#### 🎨 For Illustration (SFW, stylized):
**RenderFluid Illustration PNY (based on RealCartoon-Pony)**  
https://civitai.com/models/1830196/renderfluid-illustration-pny

This model is SFW-only and perfect for stylized characters, art, and content safe for professional use.

#### 📸 For Photo Realism (with inpainting support):
**JuggernautXL Inpainting**  
https://civitai.com/models/403361?modelVersionId=456538

Use this if you plan to run realism or detail passes for photographic content.

After downloading, place the `.safetensors` files into your ComfyUI `models/checkpoints/` folder.

---

### 🎨 Introduction to the Illustration Pipeline

The **RenderFluid Illustration Pipeline** is optimized for stylized, safe-for-work image generation using the PNY model. It’s pre-assembled, fully documented, and can be run in batches with no setup—just enter your prompt and click run.

![Example 1](_bin/rf_example_illustration_v1_0005.png)  
![Example 2](_bin/rf_example_illustration_v1_0007.png)

This workflow includes built-in prompt controls, SFW filtering, optional LoRA support, and a lightweight face detailer for improved consistency at higher resolutions.
