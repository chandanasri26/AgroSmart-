AgroSmart
AgroSmart is a starter web application for the mini project: "AgroSmart - Smart Crop Advisory and Disease Detection System."

This version implements the milestone modules end-to-end:

User registration, login, and farmer profile
Crop recommendation with an ML hook (RandomForest) and fallback logic
Fertilizer recommendation with history and nutrient status chart
Leaf disease detection with a CNN/Keras hook (when a model exists) and fallback logic
REST APIs for crop, fertilizer, and disease flows
SQLite history storage for predictions and recommendations


Tech Stack
Python 3.13+
Flask
SQLite (via SQLAlchemy)


AgroSmart/
├── app.py
├── requirements.txt
├── requirements-ml.txt
├── requirements-dev.txt
├── agrosmart/
│   ├── __init__.py
│   ├── config.py
│   ├── db.py
│   ├── models.py
│   ├── routes.py
│   ├── routes_api.py
│   ├── routes_auth.py
│   ├── routes_services.py
│   ├── services/
│   │   ├── advisory.py
│   │   ├── crop_ml.py
│   │   └── disease.py
│   └── templates/
│       ├── base.html
│       ├── public_home.html
│       ├── dashboard.html
│       ├── auth/
│       └── services/
└── static/
    └── styles.css
