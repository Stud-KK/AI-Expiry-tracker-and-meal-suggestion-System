


# 🧠 AI-Powered Expiry Predictor & Meal Suggestion System

A smart food inventory web application that helps users track groceries, predicts expiry dates using machine learning, and suggests meals based on what's nearing expiry. It also promotes sustainability by recommending reuse or composting ideas for expired food.

---

## 🚀 Features

- 🧠 **AI-Based Expiry Prediction** – Predicts expiry dates for fresh produce based on condition and storage method using a trained machine learning model.
- 🍽️ **Meal Suggestions** – Recommends recipes using items close to expiry.
- 📊 **Nutritional Info via Edamam API** – Provides nutrition details for meals and ingredients.
- ♻️ **Reuse or Compost Suggestions** – Offers sustainable suggestions for expired items (e.g., sour milk → paneer, overripe fruits → compost).
- 📦 **Inventory Management** – Track grocery items with expiry, storage, and condition data.
- 🔔 **SMS Notifications** – Sends expiry alerts via Twilio SMS.
- 🗣️ **Voice-Based Entry** – Allows users to input items via speech.
- 📈 **Inventory Analytics** – Provides charts and summaries using Python-based visualization.

---

## 🧠 Machine Learning Model

- **Model**: [XGBoost Regressor](https://xgboost.readthedocs.io/)
- **Dataset**: 500+ samples with:
  - `Product Name` (e.g., methi, milk, coriander)
  - `Storage Condition` (room temp, fridge, freezer)
  - `Item Condition` (fresh, okay, slightly spoiled)
- **Target**: Number of days before the item expires
- **Evaluation Metric**: Mean Absolute Error (MAE)
- **Performance**: Achieved MAE of ~3 days

🔍 This model is especially useful for fresh items that don’t come with printed expiry dates. By analyzing how storage and condition affect longevity, the model helps users reduce food waste and make informed decisions.

---

## 🧰 Tech Stack

| Layer           | Technology              |
|------------------|-------------------------|
| Frontend         | React.js                |
| Backend          | Node.js + Express       |
| Database         | MongoDB                 |
| ML API           | Flask (Python)          |
| ML Libraries     | XGBoost, scikit-learn   |
| Voice Input      | Web Speech API          |
| Charts           | Matplotlib, Seaborn     |
| Alerts           | Twilio SMS              |
| Recipes & Nutrition | Edamam API           |

---

## 📂 Folder Structure

```

expiry-tracker-app/
├── frontend/       # React frontend
├── backend/        # Express server (Node.js)
├── ml-api/         # Flask app with ML model
├── dataset/        # Model training data
└── README.md

````

---

## 📈 Use Case Example

> **Item Added**: Methi  
> **Condition**: Fresh  
> **Storage**: Fridge  

🔹 **Prediction**: 5 days before expiry  
🔹 **Suggestions**:
  - Meal: Aloo Methi *(via Edamam API)*
  - Nutrition: Calories, carbs, protein, etc.
  - Storage Tip: Wrap in paper to extend freshness by 2–3 days  
🔹 **If Expired**:
  - Suggestion: Use for compost/fertilizer

---

## ⚙️ Running the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/expiry-tracker-app.git
````

### 2. Install Dependencies

#### Backend & Frontend

```bash
cd backend
npm install
cd ../frontend
npm install
```

#### ML API

```bash
cd ../ml-api
pip install -r requirements.txt
```

### 3. Start Services

#### React frontend

```bash
cd frontend
npm start
```

#### Node.js backend

```bash
cd ../backend
nodemon index.js
```

#### Flask ML API

```bash
cd ../ml-api
python app.py
```

---

## 🌱 Future Improvements

* 📷 Add support for barcode scanning and image-based input
* 🌡️ Include environmental data (humidity, temperature) to refine predictions
* 🗣️ Add multilingual support for voice commands
* 🧠 Train with larger and more diverse datasets
* 📦 Integrate grocery APIs for automated entry

---

## 📜 License

This project is open-source and free to use under the MIT License.

---

## ✨ Acknowledgements

* [XGBoost](https://xgboost.readthedocs.io/)
* [Twilio](https://www.twilio.com/)
* [React](https://reactjs.org/)
* [Node.js](https://nodejs.org/)
* [MongoDB](https://www.mongodb.com/)
* [Flask](https://flask.palletsprojects.com/)
* [Edamam API](https://developer.edamam.com/) – for recipe and nutrition suggestions






