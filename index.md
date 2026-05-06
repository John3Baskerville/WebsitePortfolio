<style>
/* ── Fixed left sidebar navigation ── */
.quick-nav {
  position: fixed;
  left: max(1rem, calc((100vw - 74rem - 300px) / 4));
  top: 50%;
  transform: translateY(-50%);
  width: 150px;
  background: #fff;
  border: 1px solid #dde;
  border-radius: 8px;
  padding: 1rem;
  box-shadow: 0 2px 12px rgba(0,0,0,0.08);
  z-index: 999;
}
.quick-nav .nav-label {
  display: block;
  font-size: 0.68rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.07em;
  color: #888;
  margin-bottom: 0.6rem;
}
.quick-nav a {
  display: block;
  font-size: 0.8rem;
  color: #159957;
  text-decoration: none;
  padding: 0.28rem 0;
  border-bottom: 1px solid #f2f2f2;
}
.quick-nav a:last-child { border-bottom: none; }
.quick-nav a:hover { color: #0d6840; text-decoration: underline; }
/* Only show sidebar when there's room beside the content area */
@media (max-width: 1600px) { .quick-nav { display: none; } }

/* ── Widen Jekyll Cayman content column ── */
.main-content { max-width: 74rem !important; }

/* ── Contact row ── */
.contact-row {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem 1.6rem;
  align-items: center;
  margin-top: 0.6rem;
}
.contact-row a,
.contact-row span {
  white-space: nowrap;
  font-size: 0.92rem;
  color: #159957;
  text-decoration: none;
}
.contact-row a:hover { text-decoration: underline; }

/* ── Profile photo ── */
.profile-wrap {
  float: right;
  margin: 0 0 1.2rem 1.5rem;
  text-align: center;
}
.profile-pic {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid #159957;
  display: block;
}
.profile-placeholder {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background: #f0faf4;
  border: 2px dashed #159957;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.7rem;
  color: #159957;
  text-align: center;
  line-height: 1.5;
}
</style>

<!-- Fixed sidebar: only visible on screens ≥ 1440px wide -->
<div class="quick-nav">
  <span class="nav-label">Projects</span>
  <a href="#spotify-song-clustering">Spotify Clustering</a>
  <a href="#playlist-name-generation-with-nlp">NLP Playlists</a>
  <a href="#league-of-legends-match-outcome-prediction">League of Legends</a>
  <a href="#used-car-price-prediction">Used Car Prices</a>
  <a href="#nyc-taxi-tip-prediction">NYC Taxi Tips</a>
</div>

## About Me

<!-- Profile photo -->
<div class="profile-wrap">
  <img src="assets/profile.png" alt="John Baskerville" class="profile-pic"
       onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
  <div class="profile-placeholder" style="display: none;">
    Add photo:<br><em>assets/profile.png</em>
  </div>
</div>

I'm a data scientist with hands-on experience building end-to-end machine learning pipelines — from raw data exploration through model deployment. My projects span clustering, regression, neural networks, and NLP, with a focus on finding practical, explainable insights from real-world datasets.

<div class="contact-row">
  <a href="mailto:john3baskerville@gmail.com">📧 john3baskerville@gmail.com</a>
  <span>📞 717-701-7793</span>
  <a href="https://www.linkedin.com/in/john-baskerville/">LinkedIn</a>
  <a href="https://github.com/John3Baskerville">GitHub</a>
  <a href="https://www.hackerrank.com/john3baskerville">HackerRank</a>
</div>

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

Built a clustering pipeline on my personal Spotify library to automatically group songs into playlists — without any manual labeling. Spotify exposes 13 quantitative [audio features](https://developer.spotify.com/discover/) per track (energy, valence, tempo, etc.); I used these as model inputs, evaluated multiple `k` values, and validated cluster quality with feature profiles (heatmaps) and violin plots that describe the generated playlists themes.

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
