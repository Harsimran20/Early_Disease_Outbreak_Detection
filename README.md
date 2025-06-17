# 🦠 Early Disease Outbreak Detection Using Social Media 📍

This project uses natural language processing (NLP) and geospatial analysis to detect potential disease outbreaks by analyzing geo-tagged social media posts (e.g., tweets). It flags health-related keywords, classifies content with machine learning, and visualizes alert zones on an interactive map.

---

## 🔍 Key Features

- 🧼 **Tweet Preprocessing**: Cleans and standardizes social media text.
- 🏷️ **Symptom Labeling**: Flags posts mentioning symptoms like "fever", "cough", etc.
- 🧠 **Logistic Regression Classifier**: Learns to distinguish health-related from non-health-related posts.
- 🌍 **Outbreak Mapping**: Displays affected zones interactively using Folium.
- 📈 **Model Evaluation**: Generates classification metrics using `scikit-learn`.

---

## 📁 Project Structure

📦 disease-outbreak-detection
│
├── 🧾 outbreak_map.html # Interactive map showing alerts
├── 📜 model_training.py # Tweet preprocessing, training, and visualization
├── 📊 sample_tweet_data.csv # Input tweet data (optional)
├── 🧠 model.pkl # Saved classifier model (optional)
├── 📝 README.md # Project documentation

---

## ⚙️ Technologies Used

- Python 3.x
- `pandas`, `re` for data handling and preprocessing
- `scikit-learn` for classification
- `folium` for geospatial visualization
- `TfidfVectorizer` for text vectorization

---

## 🧪 Workflow Summary

1. **Load Tweet Data** (with text and GPS coordinates)
2. **Clean Text** (remove punctuation, lowercase, remove URLs)
3. **Label Symptom Mentions** (based on keyword match)
4. **Train Logistic Regression Classifier**
5. **Evaluate Model Performance**
6. **Visualize Labeled Tweets on Map**

---

## 🗺️ Map Visualization

- 🟥 **Red Markers**: Tweets flagged as health-related.
- 📌 **Popups**: Show the tweet text directly on the map.
- 🌐 Map is saved as `outbreak_map.html`.

---

## 💡 Sample Applications

- 🏥 **Health Surveillance Agencies**: Early alerts for regional outbreaks.
- 📊 **Epidemiologists**: Track disease spread patterns over time.
- 🌐 **Smart Cities**: Real-time integration with health dashboards.
- 📰 **Media**: Identify trending health concerns and their locations.

---
To view Map:
import webbrowser
webbrowser.open("outbreak_map.html")
