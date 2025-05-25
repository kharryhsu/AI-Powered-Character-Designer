# AI-Powered-Character-Designer

This project generates AI character images and creative lore using **Stable Diffusion** for visual generation and **EdenAI’s OpenAI-based text generation API** for imaginative backstory creation.  

Users provide a prompt and a style (Realistic, Anime, or Pixel Art), and receive a **stylized portrait** with a **rich character profile** including name, traits, personality, and backstory.

---

## 📸 Screenshots

### Sample Input

`A brave knight with a mysterious past`, `Realistic`

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

- Python 3.10.16 
- Recommended: Run inside a virtual environment

### Dependencies

Install the following Python packages:

```bash
pip install -r requirements.txt
```

---

## 🚀 Deployment

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/AI-Powered-Character-Designer.git
```

### 2. Navigate to the Project Folder

```bash
cd AI-Powered-Character-Designer
```

### 3. Create Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Launch the Notebook

Open the Jupyter Notebook interface and either:

- Run the test function to generate a sample character image and lore.
- Or run the Gradio interface to open a web-based UI and input your own prompts interactively.

---

## 📌 Notes

- You must set a valid **EdenAI API key** in the headers of the `generate_lore()` function.  
  Example (recommended):
  ```python
  "Authorization": "Bearer " + os.getenv("EDENAI_API_KEY")
  ```
  Make sure to set the environment variable `EDENAI_API_KEY` before running.
- Generated assets (images and lore) are saved in the `characters/` folder with a unique ID.
- This project uses HuggingFace's `diffusers` library to run Stable Diffusion models.
- Internet access is required to:
  - Contact EdenAI’s text generation API.
  - Download model weights from HuggingFace (if not already cached).

---

## 🔮 Future Improvements

- ☁️ Cloud Integration: Upload results to cloud storage and generate download/share links.

- 📝 Expanded Lore Generation: Support multi-paragraph stories and add character dialogue options.

---

## Contributions

We welcome contributions! 🎉  
If you have ideas, suggestions, or improvements, feel free to fork this repository and submit a pull request.  
