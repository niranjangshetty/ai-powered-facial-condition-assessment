# 🧴 AI-Powered Facial Condition Analysis

> **Dermatology-inspired skin assessment tool powered by Google Gemini 2.5 and Streamlit.**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=flat&logo=streamlit&logoColor=white)](https://streamlit.io)
[![Gemini](https://img.shields.io/badge/Google%20Gemini-2.5%20Flash-4285F4?style=flat&logo=google&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![Pillow](https://img.shields.io/badge/Pillow-Image%20Processing-green?style=flat)](https://python-pillow.org)

---

## 📌 What This Project Demonstrates

A multimodal AI application that accepts a facial image and returns a structured dermatology-style assessment — built with **Google Gemini's vision capabilities** and a clean **Streamlit** interface.

| Capability | Implementation |
|---|---|
| **Multimodal AI** | Image + text prompt sent to Gemini 2.5 Flash |
| **Prompt Engineering** | Structured expert-role prompt for consistent output |
| **Image Handling** | PIL-based image loading and sidebar preview |
| **UI/UX** | Streamlit sidebar upload + main panel results |
| **API Integration** | Google Generative AI Python SDK |

---

## 🖥️ App Preview

**Workflow:**
1. Upload a clear, well-lit facial image via the sidebar
2. Click **Analyse**
3. Receive a structured skin assessment report instantly

**Sample Output Structure:**
```
1. Skin Type:              Combination
2. Overall Skin Condition: Mild dehydration with visible pores in T-zone
3. Area-wise Observations: Forehead — slight oiliness; Cheeks — dryness
4. Skin Concerns:          Mild hyperpigmentation, early fine lines
5. Recommendations:        Hyaluronic acid serum, SPF 30+ daily
6. Preventive Measures:    Hydration, diet, consistent cleansing routine
```

---

## 🏗️ Architecture

```
User Uploads Image (Streamlit Sidebar)
          │
          ▼
  PIL Image Processing
          │
          ▼
  Gemini 2.5 Flash API
  (Image + Expert Prompt)
          │
          ▼
  Structured Assessment Report
  (Rendered in Streamlit Main Panel)
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend / UI** | Streamlit |
| **AI Model** | Google Gemini 2.5 Flash Lite (multimodal) |
| **Image Processing** | Pillow (PIL) |
| **AI SDK** | `google-generativeai` |
| **Config** | Environment variable for API key |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/facial-condition-analysis.git
cd facial-condition-analysis
```

### 2. Install Dependencies

```bash
pip install streamlit google-generativeai pillow
```

### 3. Set Your Google API Key

```bash
export GOOGLE_API_KEY=your_api_key_here
```

> Get your API key from [Google AI Studio](https://aistudio.google.com/app/apikey)

### 4. Run the App

```bash
streamlit run app.py
```

---

## 🔭 Roadmap

- [ ] Add confidence indicators per observation
- [ ] Support webcam capture in addition to file upload
- [ ] Export report as PDF
- [ ] Add ingredient-level product recommendations
- [ ] Multi-language report output

---

## ⚠️ Disclaimer

This tool is intended for **cosmetic and informational purposes only**. It is not a substitute for professional medical or dermatological advice. Always consult a qualified dermatologist for clinical concerns.

---

## 👤 Author

**Niranjan G Shetty**
*AI Applications & Generative AI Engineering*

> Built to demonstrate practical multimodal AI application development — from prompt engineering and vision model integration through to clean, user-facing interfaces.
