# 🚀 HealthPilot AI

**HealthPilot AI** is an intelligent health and wellness assistant powered by AI. It helps users make smarter lifestyle choices by tracking food, sleep, habits, and medical insights. It uses computer vision, machine learning, and health data to offer personalized advice and promote overall well-being.

---

## 🧠 Features

### 🥗 Food Recognition & Nutrition Tracking
- Detects food items using image input (OpenCV + PyTorch)
- Estimates nutritional values and calories
- Suggests healthy alternatives and recipe ideas
- Tracks water intake, cigarette consumption, and other daily habits

### 🏥 Medical History & AI Health Insights
- Allows users to log their medical history
- Offers recommendations tailored to health conditions
- Alerts users of harmful habits or potential health concerns

### 😴 AI-Powered Sleep Optimization
- Tracks sleep hours and sleep debt
- Recommends sleep schedules based on lifestyle and patterns

---

## 🛠 Tech Stack

### Backend
- **FastAPI** for the API
- **Torch**, **OpenCV**, **Pillow** for food recognition
- **Google OAuth2** for authentication
- **Pydantic** for data validation

### Frontend
- **React Native** + **Expo** for cross-platform mobile app
- **Firebase Auth** for Google Sign-In and Email/Password login
- **Firestore / SQLite** for persistent data

---

## 📁 Project Structure

### 📁 Project Structure

```
HealthPilot-AI/
├── Backend/
│   ├── app.py                # FastAPI server and endpoints
│   ├── meal_planner.py       # Food analysis and nutrition logic
│   ├── data/                 # Model or asset data
│   └── credentials.json      # Google OAuth credentials
│
├── Frontend/
│   ├── src/                  # React Native frontend source code
│   ├── assets/               # Icons and images
│   └── App.tsx               # Root of React Native app
│
├── requirements.txt          # Backend Python dependencies
└── app.json                  # Expo config for React Native
```


---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js & npm
- Python 3.8+
- Expo CLI (`npm install -g expo-cli`)
- Firebase project set up (for auth + DB)

---

### 🔧 Installation Steps

#### 1. Clone the Repository
```bash
git clone https://github.com/your-username/healthpilot-ai.git
cd healthpilot-ai
```

2. Install Backend Dependencies
```
cd Backend
pip install -r requirements.txt
```

3. Set up Firebase
```
Add your Firebase credentials to Frontend/firebaseConfig.js
```

4. Start Backend Server
```
uvicorn app:app --reload
```

5. Install Frontend Dependencies
```
cd ../Frontend
npm install
```

6. Start React Native App

```
expo start
```

### 💡 Future Improvements
-Real-time fitness tracking with wearables

-Integration with Apple Health / Google Fit

-In-app chat support with AI health assistant

-Mental wellness & mood tracking features


### 📜 License

This project is licensed under the MIT License.
