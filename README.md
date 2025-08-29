# Your Text, Your Style – Auto-Generate a Presentation

A web app that transforms bulk text, markdown, or long-form prose into a fully formatted PowerPoint presentation that matches the style, layout, and images of an uploaded template.

---

## ✨ Features

* Paste or type in large blocks of text (supports markdown & prose)
* Add optional one-line guidance (e.g., *"turn into an investor pitch deck"*)
* Upload a PowerPoint template or presentation (`.pptx` or `.potx`)
* Provide your own LLM API key (OpenAI, Anthropic, Gemini, etc.) – **never stored or logged**
* App analyzes and splits input text into structured slide content
* Reuses template’s images, colors, fonts, and layouts
* Outputs a new PowerPoint presentation (`.pptx`) ready for download

---


---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/auto-ppt-generator.git
cd auto-ppt-generator
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the App

```bash
python run.py
```

The app will be available at: `http://localhost:5000`

---

## 🔑 API Key Setup

* You must provide your own LLM API key.
* The app supports **OpenAI, Anthropic, and Gemini**.
* The key is **used only in your session** and never stored.

---

## 🛠️ How It Works

1. User pastes bulk text or markdown
2. User uploads `.pptx` or `.potx` template file
3. App parses the template’s **style, fonts, layouts, and images**
4. LLM processes text → slide titles, bullet points, structure
5. Content mapped onto template layout
6. New `.pptx` file generated and made available for download

---

## 📦 Dependencies

* Python 3.9+
* Flask (or FastAPI)
* python-pptx
* requests
* Any LLM SDK (OpenAI, Anthropic, Google Gemini)

---

## 📖 Example Usage

1. Paste in this text:

   ```
   Artificial Intelligence is transforming industries...
   ```
2. Upload a **corporate pitch deck template**
3. Enter API key & click **Generate Presentation**
4. Download the finished `.pptx` styled with your chosen theme

---

## 📜 License

MIT License. See [LICENSE](./LICENSE) for details.

---



## 🌍 Deployment

* Can be deployed to **Heroku, Render, Vercel, or AWS**
* Ensure environment variable `API_PROVIDER` and `API_KEY` are set when running in production

---

## 👨‍💻 Author

Developed with ❤️ by Rahul Burdak
