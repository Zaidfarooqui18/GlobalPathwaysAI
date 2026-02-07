# 🌍 Global Pathways AI
A neutral, AI-powered decision engine that helps students decide between studying locally or abroad. Features a custom ROI calculator, visa probability estimation, and a comparison matrix to eliminate agent bias.
**Plan your education and career with data, not guesswork.**

Global Pathways AI is a transparency-first decision support platform designed to help graduates and early-career professionals answer one core question: *Should I stay local or go abroad?*

Unlike traditional counseling agents driven by commissions, our "Neutral AI Advisor" uses machine learning to provide unbiased recommendations based on your budget, career goals, and risk appetite.

## 🚀 Live Demo
- **Frontend:** [https://global-pathways-ai.vercel.app/](https://global-pathways-ai.vercel.app/)
- **Backend API:** [https://case-study-global-pathways-ai.onrender.com](https://case-study-global-pathways-ai.onrender.com)
- **Figma Prototype:** [View Design Workflow](https://www.figma.com/design/cuUXmaN9P6PGYdEI6Zrnov/workflow?node-id=0-1&t=jUdqLDcA9wH3cdkl-1)

---

## ✨ Key Features

* **🤖 Dual-Layer AI Prediction:**
    * **Pathway Model:** Binary classifier (Study Local vs. Abroad).
    * **Destination Model:** Ranks top 3 countries based on profile fit.
* **💰 Smart ROI Calculator:** Custom metric combining tuition, living costs, and projected 3-year salary to quantify financial outcomes.
* **🛂 Visa Probability Engine:** Estimates Permanent Residency (PR) success rates based on country policies.
* **📊 Comparison Matrix:** Side-by-side view of tuition, living expenses, and visa chances for multiple countries.
* **✅ Transparency Checklist:** "Why this is recommended" breakdown for every result.

---

## 🛠️ Tech Stack

### **Frontend (User Interface)**
* **Framework:** React.js (Vite)
* **Styling:** CSS3 (Modular & Responsive)
* **State Management:** React Hooks (`useState`)
* **Architecture:** Single Page Application (SPA)

### **Backend (Intelligence)**
* **Language:** Python
* **ML Libraries:** CatBoost, Scikit-learn, Pandas
* **NLP:** SentenceTransformers (`all-MiniLM-L6-v2`) for intent parsing
* **Deployment:** Render

---

## 🧠 The AI Architecture

The system utilizes a **CatBoost Classifier**, chosen for its superior handling of categorical variables (like "Field of Study" or "Degree Type") without the need for extensive preprocessing.

1.  **Input Layer:** User provides Budget ($20k-$40k), Field (CS/Data), and Timeline.
2.  **Processing Layer:**
    * *Pathway Predictor* determines the optimal route.
    * *ROI Engine* calculates financial viability.
3.  **Output Layer:** Returns a ranked list of destinations with confidence scores (e.g., "Canada: 78% Match").

---

## 🏃‍♂️ Running Locally

### **Frontend Setup**
```bash
# Clone the repository
git clone [https://github.com/yashfeenraavi09/globalpathways.git](https://github.com/yashfeenraavi09/globalpathways.git)

# Navigate to the frontend directory
cd frontend

# Install dependencies
npm install

# Run the development server
npm run dev

### **Backend Setup**
```bash
# Navigate to the backend directory
cd backend

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py
