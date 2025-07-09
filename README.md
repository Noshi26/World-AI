🌐 WorldWatch AI: The Definitive Intelligence Engine
![alt text](https://img.shields.io/badge/Python-3.9+-blue.svg)

![alt text](https://img.shields.io/badge/License-MIT-yellow.svg)

![alt text](https://colab.research.google.com/assets/colab-badge.svg)
WorldWatch AI is a real-time geopolitical intelligence dashboard that uses AI to monitor, analyze, and visualize global events from news sources. It transforms the overwhelming stream of public information into structured, actionable insights.
This project is contained within a single, fully-functional Jupyter/Colab notebook. It automates the entire intelligence pipeline: from data ingestion and NLP-based classification to machine learning-powered forecasting and interactive visualization.
Dashboard Preview
(Note: You should replace this with an actual screenshot of your running dashboard)
A preview of the AI Economic Advisor and News Feed tabs.
✨ Key Features
📰 Automated News Aggregation: Ingests real-time news from global sources (via NewsAPI) and specific regional sources (Bangladeshi RSS feeds).
🧠 AI-Powered Classification: Uses a rule-based expert system and NLP to classify articles into key categories (War, Trade, Economic, Peace, Tech) and assign a quantitative risk score.
🌍 Interactive Threat Map: Geocodes events using spaCy and geopy to plot them on an interactive world map, visualizing hotspots of geopolitical activity.
📈 Dynamic Trend Analysis: Aggregates risk scores over time to create interactive trend charts, showing the rise and fall of different risk categories and forecasting near-term activity.
💰 Market Pulse & Correlation: Fetches live market data (S&P 500, Gold, Oil) and correlates significant geopolitical events with market price action.
🛰️ Event Path Simulation (A* Search): Simulates a plausible sequence of news events that could lead from a Stable geopolitical state to Active Conflict, demonstrating a classic AI state-space search algorithm.
🤖 AI Economic Advisor: The core analytical feature—a machine learning model (RandomForestClassifier) trained on historical news risk and market volatility (VIX) to predict the near-term economic outlook and identify its key drivers.
🛠️ Technology Stack
The entire project is built with Python and leverages a powerful stack of data science and AI libraries:
Core AI & NLP:
scikit-learn: For training the Random Forest classification model.
spaCy: For advanced Natural Language Processing, specifically Named Entity Recognition (NER) to geolocate news.
vaderSentiment: For sentiment analysis (used implicitly in the keyword scoring).
Data Handling & Sourcing:
pandas: For data manipulation and analysis.
numpy: For numerical operations.
yfinance: For fetching historical and real-time stock market data.
feedparser: For parsing RSS news feeds.
Visualization & UI:
ipywidgets: To create the interactive dashboard components (tabs, buttons, dropdowns).
plotly: For creating beautiful, interactive charts and graphs.
folium: For rendering the interactive world map.
Environment:
Jupyter / Google Colab: The interactive development environment.
🚀 Getting Started
This project is designed to be run with a single click in Google Colab.
Prerequisites
A web browser.
A Google Account (for using Google Colab).
A NewsAPI key (it's free for developers).
Installation & Usage
Open the Notebook in Colab:
Click the "Open in Colab" badge at the top of this README.
Add Your API Key:
Inside the Colab notebook, find this line of code:
Generated python
NEWS_API_KEY = "6db142084e204cde87768c6b635fb67e"
Use code with caution.
Python
Replace the placeholder key with your own free key from newsapi.org.
Run the Code:
Execute the single code cell in the notebook by clicking the "Play" button next to it or by pressing Shift + Enter.
The cell will first install all required libraries (this may take a minute or two).
After installation, it will run the pipeline and display the fully interactive dashboard directly in the cell output.
🤖 AI Methodology Breakdown
WorldWatch AI showcases a composite AI system, integrating several core AI concepts:
Knowledge Representation & Rule-Based Reasoning: The system uses a hand-crafted knowledge base (UPGRADED_KEYWORDS) where keywords are weighted. An inference engine (classify_text function) applies these rules to classify news, mimicking an expert system.
Natural Language Processing (NLP): spaCy is used to perform semantic analysis on unstructured text. Its Named Entity Recognition (NER) model is crucial for extracting geopolitical entities (countries, cities) to enable geographic visualization.
State-Space Search: The "Event Tracker" uses the A* search algorithm to find the optimal path from a start state (Stable) to a goal state (Active Conflict) by navigating through the graph of news events and predefined state transitions.
Inductive Learning (Machine Learning): The "AI Economic Advisor" employs a supervised learning model (RandomForestClassifier) that learns the complex, non-linear relationship between aggregated daily news risk and real-world market volatility. It then uses this learned knowledge to make probabilistic forecasts on new data.
📜 License
This project is licensed under the MIT License. See the LICENSE file for details.
👤 Contact
Noshi26 - GitHub Profile
Project Link: https://github.com/Noshi26/World-AI
