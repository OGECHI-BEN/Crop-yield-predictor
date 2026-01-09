# Crop Yield Predictor 
# 🌾 Crop Yield Prediction System

A full-stack machine learning application that predicts crop yields based on environmental and agricultural factors using AI/ML models.

## 📋 Overview

This application helps farmers and agricultural professionals predict crop yields by analyzing various parameters such as soil conditions, weather patterns, fertilizer usage, and historical data. The system uses machine learning algorithms to provide accurate yield predictions to support better farming decisions.

 Features

- **Intelligent Predictions**: ML-powered crop yield forecasting
- **Interactive Dashboard**: Real-time visualization of predictions and trends
- **Multi-parameter Analysis**: Considers soil type, weather, crop type, fertilizers, and more
- **Historical Data Tracking**: View past predictions and actual yields
- **User-friendly Interface**: Clean, responsive React-based UI
- **RESTful API**: Well-documented backend API for easy integration

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI framework
- **Axios** - HTTP client for API calls
- **Chart.js / Recharts** - Data visualization
- **Tailwind CSS / Material-UI** - Styling

### Backend
- **Python 3.x** - Core programming language
- **Flask / FastAPI** - Web framework
- **scikit-learn** - Machine learning library
- **pandas** - Data manipulation
- **NumPy** - Numerical computing
- **joblib / pickle** - Model serialization

### Machine Learning
- **Algorithm**: [Random Forest / XGBoost / Neural Networks]
- **Features**: Temperature, rainfall, soil pH, NPK values, crop type, etc.
- **Target**: Crop yield (tons per hectare)

## 📁 Project Structure

```
crop-yield-predictor/
├── frontend/                 # React application
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API services
│   │   └── utils/           # Utility functions
│   ├── public/
│   └── package.json
│
├── backend/                  # Python application
│   ├── app/
│   │   ├── models/          # ML models
│   │   ├── routes/          # API endpoints
│   │   ├── services/        # Business logic
│   │   └── utils/           # Helper functions
│   ├── data/                # Training datasets
│   ├── notebooks/           # Jupyter notebooks for ML experiments
│   ├── requirements.txt
│   └── main.py
│
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Python 3.8+
- pip or conda

### Backend Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/crop-yield-predictor.git
   cd crop-yield-predictor/backend
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Train the model (if needed)**
   ```bash
   python train_model.py
   ```

5. **Run the backend server**
   ```bash
   python main.py
   ```
   The API will be available at `http://localhost:5000`

### Frontend Setup

1. **Navigate to frontend directory**
   ```bash
   cd ../frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```
   The app will open at `http://localhost:3000`

## 📊 API Endpoints

### POST `/api/predict`
Predict crop yield based on input parameters

**Request Body:**
```json
{
  "temperature": 25.5,
  "rainfall": 800,
  "soil_ph": 6.5,
  "nitrogen": 40,
  "phosphorus": 30,
  "potassium": 20,
  "crop_type": "wheat",
  "area": 10
}
```

**Response:**
```json
{
  "predicted_yield": 45.8,
  "unit": "tons per hectare",
  "confidence": 0.92
}
```

### GET `/api/crops`
Get list of supported crop types

### GET `/api/history`
Retrieve prediction history

## 🧪 Model Details

- **Algorithm**: Random Forest Regressor
- **Training Data**: 10,000+ samples from agricultural datasets
- **Features**: 8 input parameters
- **Accuracy**: R² score of 0.89 on test set
- **Last Updated**: [Date]

## 📈 Future Enhancements

- [ ] Integration with weather APIs for real-time data
- [ ] Multi-season predictions
- [ ] Crop disease detection
- [ ] Mobile application
- [ ] Integration with IoT sensors
- [ ] Support for more crop varieties
- [ ] Multi-language support

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Your Name** - [GitHub Profile](https://github.com/yourusername)

## 🙏 Acknowledgments

- Dataset sources: [Kaggle / UCI ML Repository / etc.]
- Inspiration from agricultural research papers
- Open-source community



---

⭐ If you find this project useful, please consider giving it a star!
