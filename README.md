# 🛡️ PhishGuard - AI Phishing URL Detection & Explainable AI Engine

![License](https://img.shields.io/badge/License-MIT-emerald.svg)
![ML Precision](https://img.shields.io/badge/Model_Precision-98.4%25-cyan.svg)
![XAI Engine](https://img.shields.io/badge/XAI_Framework-SHAP_Style-indigo.svg)
![Status](https://img.shields.io/badge/Deployment-GitHub_Pages-brightgreen.svg)

> **PhishGuard** is an open-source, client-side Machine Learning URL Feature Extraction and Explainable AI (XAI) security dashboard designed to detect phishing landers, typosquatting domains, and credential harvesting links in real time.

---

## ⚡ Key Features

- **Live URL Scanner**: Scans target links in < 5ms using client-side feature extraction.
- **20 Signal Feature Vector Engine**: Extracts lexical metrics, Shannon entropy, protocol security, IPv4 host presence, subdomain depth, high-risk TLDs, and IDN homographs.
- **Ensemble ML Classifier**: Weighted Logistic Ensemble yielding a **Threat Risk Index (0 - 100%)**.
- **Explainable AI (XAI)**: Visual SHAP-style feature impact breakdown chart and plain-English anomaly explanations.
- **Batch Analyzer & CSV Export**: Audit multiple URLs concurrently and export downloadable CSV security reports.
- **Interactive Model Training Lab**: Inspect model Accuracy (98.4%), Precision (97.8%), Recall (98.9%), ROC Curve (AUC = 0.992), and tune feature weights live.

---

## 🎯 Detection Pipeline Architecture

```
User Enters URL
       ↓
URL Feature Extractor (20 Signals)
       ↓
Feature Vector Normalization
       ↓
ML Model Prediction (Sigmoid Logistic Ensemble)
       ↓
┌───────────────────────────────────────────────┐
│ Legitimate (0-30%)  │  Phishing Risk (70-100%)│
└───────────────────────────────────────────────┘
       ↓
Threat Risk Score + SHAP-Style Explanation
```

---

## 🚀 Live Demo & Hosting

You can host this project completely free using **GitHub Pages**:

1. Upload repository files to GitHub.
2. Go to **Settings → Pages**.
3. Under **Branch**, select `main` and root folder `/`.
4. Click **Save**. Your site will be live at `https://<your-username>.github.io/<repository-name>/`.

---

## 🛠️ Project Structure

```
phishing-url-detector/
├── index.html              # Main Single-Page Application
├── README.md               # Documentation & Setup Guide
├── css/
│   └── style.css           # Glassmorphism Cyber Theme
└── js/
    ├── featureExtractor.js # 20 Signal Feature Extractor
    ├── mlClassifier.js     # Weighted Ensemble ML Classifier
    ├── xaiEngine.js        # SHAP-Style Explainable AI Engine
    ├── sampleUrls.js       # Preset Test Suite & Batch Data
    └── app.js              # Application Logic & Event Handlers
```

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
