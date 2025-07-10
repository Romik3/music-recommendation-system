# 🎵 Music Recommendation System

A content-based filtering system that recommends music based on audio features using machine learning. The system also uses dimensionality reduction (t-SNE) to visualize song similarities.

---

## 🎯 Objective

To build a music recommendation system that:
- Suggests songs based on content-based filtering using audio features.
- Visualizes song similarities using dimensionality reduction techniques like t-SNE.

---

## 🧠 Theory

In the era of vast digital music libraries (e.g., Spotify), users often struggle to find songs that match their preferences. This project uses:
- **Audio-based features** (like danceability, energy, tempo)
- **Cosine similarity** to find similar songs
- **t-SNE** for 2D visualization of song clusters

---

## 📊 Dataset Description

The dataset (from Spotify or similar sources) contains ~50,000 tracks, each with attributes such as:

- `name`, `artist`, `release_date`
- `danceability`, `energy`, `valence`, `tempo`, `acousticness`
- `popularity`, `speechiness`, `liveness`, etc.

---

## 🛠 Tools & Libraries Used

- `pandas` – Data manipulation
- `numpy` – Numerical computation
- `matplotlib`, `seaborn` – Data visualization
- `scikit-learn` – Scaling, cosine similarity, t-SNE

---

## 🚦 Procedure

1. **Load and explore data**  
   Check for nulls, duplicates, and drop irrelevant columns.

2. **Feature scaling**  
   Use `StandardScaler` to normalize numerical features.

3. **Visualize with t-SNE**  
   Reduce dimensions to 2D and plot song clusters.

4. **Content-based filtering**  
   Use cosine similarity to compute similarity scores.

5. **Recommendation function**  
   Given a song name, find and rank similar songs by similarity and popularity.

---

## 🔍 Example Usage

```python
recommend_songs('Shape of You')
recommend_songs('rockstar')
