# End-to-End-Recipe-Recommendation-System-using-Flask-and-Machine-Learning
📖 Overview

This project is an end-to-end web-based Recipe Recommendation System that suggests the most relevant recipes based on ingredients and nutritional values such as calories, fat, carbohydrates, protein, and more.
It combines TF-IDF Vectorization (for text-based ingredient similarity) and K-Nearest Neighbors (KNN) (for numeric feature similarity) to provide intelligent, personalized recipe recommendations.

The system is deployed using Flask, allowing real-time user interaction through a simple and interactive web interface.

🚀 Features

🥗 Hybrid Recommendation Model: Combines text (ingredients) and numeric (nutritional) similarity.

⚙️ Machine Learning Integration: Uses TF-IDF and KNN (Euclidean Distance) for recipe matching.

💻 Web Interface: Built using Flask, with easy input forms for ingredients and nutritional values.

📊 End-to-End Pipeline: Includes preprocessing, model building, and live prediction.

📷 Image Integration: Displays recipe images fetched from the dataset.

🧠 Tech Stack
Category	Tools / Libraries
Language	Python
Framework	Flask
Machine Learning	Scikit-learn (TF-IDF, KNN, StandardScaler)
Data Handling	Pandas, NumPy
Frontend	HTML, CSS, Bootstrap
Dataset	recipe_final.csv (contains recipe names, nutritional data, ingredients, and image URLs)
📂 Project Structure
📦 Recipe_Recommendation_System
│
├── app.py                    # Main Flask application
├── recipe_final.csv          # Recipe dataset
├── templates/
│   └── index.html            # Frontend HTML file
├── static/
│   └── style.css             # CSS styling (optional)
├── recipe_recommendation_system.ipynb  # Model development notebook
└── README.md                 # Project documentation

⚙️ How It Works

Input:
User enters nutritional values (calories, fat, carbs, protein, etc.) and a list of ingredients.

Processing:

The system vectorizes the ingredients using TF-IDF.

Scales the numeric features using StandardScaler.

Combines both types of data into one feature vector.

Model:
A K-Nearest Neighbors (KNN) model finds the most similar recipes based on Euclidean distance.

Output:
The app displays top 5 recommended recipes with names, ingredients, and image links.

💻 Installation and Setup
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/Recipe-Recommendation-System.git
cd Recipe-Recommendation-System

2️⃣ Install Dependencies

Make sure you have Python 3.8+ installed.

pip install -r requirements.txt


(If you don’t have a requirements file, you can create one with:)

pip freeze > requirements.txt

3️⃣ Run the Flask App
python app.py

4️⃣ Open in Browser

Visit:

http://127.0.0.1:5000/


You’ll see the home page where you can enter inputs and get recipe recommendations instantly.

📊 Example Input
Feature	Example Value
Calories	250
Fat	10
Carbohydrates	30
Protein	12
Cholesterol	20
Sodium	150
Fiber	5
Ingredients	chicken, garlic, butter
🎯 Example Output

Top 5 recipes with:

Recipe Name

Ingredients List

Image Preview

📈 Future Enhancements

Add user login and personalized recommendation history.

Integrate image-based recipe search using deep learning (CNN).

Deploy the system on Render / AWS / Hugging Face Spaces.

Add ratings and reviews for user feedback.

👨‍💻 Author

Md Imran Akhtar
🔗 GitHub
 • LinkedIn

🏁 Outcome Highlights

Built and deployed a complete ML-powered recommendation system from scratch.

Combined TF-IDF + KNN for hybrid similarity-based recipe matching.

Delivered an interactive and scalable Flask application for real-world use.
