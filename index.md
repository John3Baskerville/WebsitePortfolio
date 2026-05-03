## About Me

I'm a data scientist with hands-on experience building end-to-end machine learning pipelines — from raw data exploration through model deployment. My projects span clustering, regression, neural networks, and NLP, with a focus on finding practical, explainable insights from real-world datasets.

📧 [john3baskerville@gmail.com](mailto:john3baskerville@gmail.com) &nbsp;|&nbsp; 📞 717-701-7793 &nbsp;|&nbsp; [LinkedIn](https://www.linkedin.com/in/john-baskerville/) &nbsp;|&nbsp; [GitHub](https://github.com/John3Baskerville) &nbsp;|&nbsp; [HackerRank](https://www.hackerrank.com/john3baskerville)

---

## Skills

| Area | Tools & Technologies |
|---|---|
| Languages | Python, SQL |
| Machine Learning | scikit-learn, Keras / TensorFlow, Logistic Regression, Neural Networks |
| Data Science | Pandas, NumPy, Matplotlib, Seaborn, Jupyter |
| Techniques | Unsupervised Clustering, NLP / Topic Modeling, Feature Engineering, Model Evaluation |

---

## Projects

### Spotify Song Clustering
**Unsupervised ML · Clustering · Spotify API · Python**

Built a clustering pipeline on my personal Spotify library to automatically group songs into playlists — without any manual labeling. Spotify exposes 13 quantitative [audio features](https://developer.spotify.com/discover/) per track (energy, valence, tempo, etc.); I used these as model inputs, evaluated multiple `k` values, and validated cluster quality with silhouette scores.

**Key takeaway:** The model surfaced musically coherent groupings that aligned well with my own listening intuition, demonstrating that unsupervised methods can learn meaningful structure from audio feature spaces.

[View Project →](https://john3baskerville.github.io/SpotifyClustering/)

---

### Playlist Name Generation with NLP
**NLP · Topic Modeling · Python**

Extended the clustering project above by treating each cluster's song titles as a text corpus and applying topic modeling to generate a descriptive name for each playlist. This closes the loop on the end-to-end pipeline: raw audio features → clusters → human-readable playlist labels.

[View Notebook →](https://github.com/John3Baskerville/SpotifyClustering/blob/main/Juypter%20Notebooks/NLP%20Topic%20Generation%20Spotify%20Songs.ipynb)

---

### League of Legends Match Outcome Prediction
**Classification · Logistic Regression · Neural Networks · Python**

Used a dataset of 10,000 ranked matches to predict the winning team from in-game statistics captured at the 10-minute mark. Performed feature importance analysis to identify the most predictive early-game signals, then compared a baseline logistic regression model against a multi-layer neural network.

[Logistic Regression Model →](https://htmlpreview.github.io/?https://github.com/John3Baskerville/LeagueOfLegendsMatchMLAnalysis/blob/main/LogisticRegressionLOLPrediction.html) &nbsp;|&nbsp; [Neural Network Model →](https://htmlpreview.github.io/?https://github.com/John3Baskerville/LeagueOfLegendsMatchMLAnalysis/blob/main/LOLMLPrediction%20.html)

---

### Used Car Price Prediction
**Regression · Feature Engineering · Python**

Trained a linear regression model to predict used car prices from vehicle attributes. Focused on preprocessing and feature selection to improve model interpretability alongside predictive accuracy.

[View Project →](https://github.com/John3Baskerville/UsedCarPriceLinearRegression)

---

### NYC Taxi Tip Prediction
**Regression · Neural Networks · Python · Public Dataset**

Analyzed NYC Taxi and Limousine Commission trip data to help drivers forecast tip percentages for airport pickups. Built and compared regression and neural network models, identifying the fare and trip features most predictive of tip behavior.

[View Notebook →](https://htmlpreview.github.io/?https://github.com/John3Baskerville/NYC-TLC-Tip-Percentage-Prediction/blob/main/Tip%20Percent%20NN%20and%20Regression.html)
