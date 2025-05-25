# AI-Powered-Character-Designer

This project generates AI character images and creative lore using **Stable Diffusion** for visual generation and **EdenAI’s OpenAI-based text generation API** for imaginative backstory creation.  

Users provide a prompt and a style (Realistic, Anime, or Pixel Art), and receive a **stylized portrait** with a **rich character profile** including name, traits, personality, and backstory.

---

## 📸 Screenshots

### Sample Output

#### Character Image (Realistic Style)

#### Character Lore

---

## ✨ Features

- 🎨 **Image Generation**  
  Uses `runwayml/stable-diffusion-v1-5` via HuggingFace `diffusers` to generate high-quality character portraits.

- ✍️ **Text Generation**  
  Connects to EdenAI’s OpenAI backend to create rich character profiles (name, traits, personality, backstory).

- ⚙️ **Custom Style Support**  
  Select from **Realistic**, **Anime**, or **Pixel Art** styles.

- 💾 **Auto Save**  
  Each generated character's image and lore are saved locally in the `characters/` folder with a UUID.

- 🧠 **GPU Acceleration**  
  Automatically uses **CUDA** if available for faster image generation.

---

## ⚙️ Requirements

- Python 3.x  
- Recommended: Run inside a virtual environment

### Dependencies

Install the following Python packages:

```bash
pip install -r requirements.txt
```

---

## 🚀 Deployment
