# 🚗⚡ AIEVCompass – AI-Powered Electric Vehicle Consultant
### *Shell – Edunet Foundation – AICTE Green Skill Internship Project*

AIEVCompass is an end-to-end **AI-powered EV consulting system** using a unique **Hybrid AI "Two-Brain" Architecture"**:

- 🧠 **Language Brain (DialoGPT-small)** — Conversational AI that interviews users  
- 🔢 **Math Brain (Expert ML Engine)** — Price & Range predictions using feature engineering  

The system predicts:

- **EV Price** (Customer Mode — 13 engineered features)  
- **EV Range** (Company Mode — 66 engineered features)  
- **Market Segment** (Budget / Mid / Premium / Luxury)

---

## 🧠 Hybrid AI Architecture

### 1️⃣ **Language Brain — Conversational AI**
Powered by **DialoGPT-small**, it extracts features naturally from user text:
> “I want a 400 km range EV” → Range = 400  
> “Top speed around 200” → Top_Speed = 200  

### 2️⃣ **Math Brain — Expert ML Engine**
Includes two modules:

#### **Customer Mode – Price Prediction**
Uses 7 user-given inputs → engineered into 13 ML features.

#### **Company Mode – Range Prediction**
Uses 8 engineering inputs → converted into a 66-feature vector.

Both run inside Streamlit via a custom UI.

---

## 🧰 Technology Stack

| Component | Tools |
|----------|-------|
| ML Models | Random Forest |
| LLM | transformers, DialoGPT-small, PyTorch |
| Frontend | Streamlit |
| Notebooks | Jupyter, matplotlib, seaborn |
| Deployment | HuggingFace |

---

## 🗂 Project Structure

```plaintext
AIEVCompass/
│
├── AIEVCompass_Dataset/
│   ├── cars_data_RAW.csv
│   └── cars_data_cleaned.csv
│
├── models/                      
│   ├── price/
│   └── range/
│
├── app/
│   └── app.py                   
│
├── notebooks/
│   ├── AIEVCompass.ipynb
│   └── Chatbot_Playground.ipynb
│
├── requirements.txt
└── README.md
````

---

## 💬 Conversation Modes

### **Customer Mode (Price Prediction)**

Chatbot collects:

* Range
* Battery
* Top Speed
* Acceleration
* Fast Charging
* Brand
* Drive Type

Models return:

* **Estimated Price ($)**
* **Market Segment (Budget → Luxury)**

---

### **Company Mode (Range Prediction)**

Chatbot collects:

* Battery
* Top Speed
* Efficiency
* Fast Charging
* Brand
* Model Name
* Drive Type
* Tow Hitch

Models return:

* **Estimated Range (km)**
* **Range Category (Very Short → Very Long)**

---

## 🏃 How to Run

### 1️⃣ Clone the repository

```bash
git clone https://github.com/charantej385/AIEVCompass-AI-powered-.git
cd AIEVCompass-AI-Powered-EV-Consultant-
```

### 2️⃣ Create a virtual environment

```bash
python -m venv venv
```

**Windows:**

```bash
.\venv\Scripts\activate
```

**Linux/Mac:**

```bash
source venv/bin/activate
```

### 3️⃣ Install requirements

```bash
pip install -r requirements.txt
```

### 4️⃣ Download DialoGPT-small

Place it at:

```
C:\DialoGPT-small
```

(or update the path in `app.py`)

### 5️⃣ Run Streamlit App

```bash
streamlit run app/app.py
```

---

## 🎨 Features

* Dark themed Streamlit UI
* Sidebar navigation
* Two modes (Customer & Company)
* NLP input → Feature extraction
* Beautiful prediction cards
* Advanced engineered features
* About/Profile section

---

## 👨‍💻 Author

**V Charan tej goud**
📧 Email: *[vcharantejgoud@gmail.com](mailto:vcharantejgoud@gmail.com)*
🔗 LinkedIn: [https://www.linkedin.com/in/v-charan-tej-goud-6aa22a314/](https://www.linkedin.com/in/v-charan-tej-goud-6aa22a314/)
💻 GitHub: [https://github.com/charantej385](https://github.com/charantej385)

```
