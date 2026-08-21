# Hi, I'm Nathan Mariñas 👋

**AI / Machine Learning Engineer** focused on applied ML, data systems and production-oriented AI.

BSc in Artificial Intelligence from **Universidade da Coruña**. Previously **AI Engineer Intern at ABANCA**, working on GenAI, RAG reliability and predictive systems.

I enjoy taking projects through the full lifecycle:

**data → experimentation → evaluation → engineering → usable product**

## Selected Work

### 🚲 [BiciCoruña Fleet Optimization](https://github.com/nathanmarinas2/bicicoruna-fleet-optimization)

**Real-time Data Engineering · Machine Learning · Mobility Analytics**

End-to-end system for understanding and predicting bike availability across A Coruña's public bike-sharing network.

* Built a historical dataset from scratch by collecting GBFS telemetry every 5 minutes across **79 stations**.
* Developed a LightGBM model for 30-minute availability risk prediction.
* Achieved **F1 = 0.78** and **87% accuracy**.
* Segmented stations into behavioral archetypes using clustering.
* Converted predictions into operational fleet-rebalancing recommendations.
* Research featured by **El Español / Quincemil**.

`Python` `LightGBM` `Pandas` `Streamlit` `Railway` `Leaflet`

---

### 🎵 [Music Graph Explorer](https://github.com/nathanmarinas2/music-graph-explorer)

**Graph ML · Representation Learning · Browser-side Inference**

Interactive system for exploring relationships between artists through collaboration graphs and learned embeddings.

* Built a public graph with **100,000 artists** and **1,059,326 collaboration edges**.
* Generated Node2Vec-style graph embeddings using random walks.
* Projected 64-dimensional representations into 3D with UMAP.
* Quantized embeddings to int8 for a **6.1 MB browser-side inference bundle**.
* Built MixDNA lite and collaboration-path exploration with no backend dependency.
* Packaged the complete experience as a static web application.

`Python` `DuckDB` `Gensim` `UMAP` `JavaScript` `Three.js`

**[Live Demo →](https://nathanmarinas2.github.io/music-graph-explorer/)**

---

### ⚡ [EnergiaPredictorES](https://github.com/nathanmarinas2/EnergiaPredictorES)

**Time-Series Forecasting · ML vs Deep Learning**

Electricity demand forecasting system comparing classical ML, deep learning and statistical baselines.

* Engineered cyclical, lag, rolling-window and calendar features.
* Compared LightGBM, XGBoost, Temporal Fusion Transformer and statistical baselines.
* Best model: **LightGBM — 1.15% MAPE**.
* Reduced forecasting error by approximately **88% vs. the best statistical baseline**.
* Structured as a modular and reproducible ML pipeline.

`Python` `LightGBM` `XGBoost` `PyTorch` `Darts` `Pandas`

---

### 🌬️ [Green Energy Sentinel](https://github.com/nathanmarinas2/Green-Energy-Sentinel)

**Geospatial Analytics · Decision Systems · Renewable Energy**

GIS-based decision-support system for wind farm site suitability in Galicia.

* Combined high-resolution wind-resource layers with **40,000+ historical lightning observations**.
* Converted discrete lightning events into continuous spatial risk surfaces.
* Applied multi-criteria decision analysis to identify candidate locations.
* Validated recommendations against existing infrastructure using OpenStreetMap data.
* Built interactive geospatial and temporal visualizations.

`Python` `Rasterio` `GeoJSON` `Folium` `PyDeck` `GIS`

---

### 🚌 BUS-CO

**Product Engineering · Urban Mobility**

Real-time public transport PWA for A Coruña.

* Built the product end-to-end with a mobile-first architecture.
* Implemented local caching and Cloudflare infrastructure for near-instant route queries.
* Integrated geolocation, maps and urban mobility data.
* Designed a privacy-first client-side architecture with no third-party tracking.

`JavaScript` `Cloudflare` `Leaflet` `HTML` `CSS`

## Research

### 🔭 Deep Learning × Astrophysics

Research work with **Gaia and Euclid astronomical data**, exploring neural-network methods for stellar classification and the characterization of binary systems and substellar companions.

The work combines scientific data processing, feature engineering, model evaluation and large-scale astronomical datasets.

## Technical Stack

**Machine Learning**
Python · PyTorch · Scikit-learn · LightGBM · XGBoost · TensorFlow

**Data**
Pandas · NumPy · DuckDB · Time Series · Feature Engineering · GIS

**AI Systems**
LLMs · RAG · Context Management · Evaluation · NLP

**Engineering & Product**
Git · Docker · Linux · JavaScript · Cloudflare · Railway · Streamlit

## What I care about

* Building ML systems around **measurable outcomes**, not model complexity.
* Strong baselines and rigorous evaluation.
* Reproducible data and ML pipelines.
* Understanding failure modes and limitations.
* Turning technical work into products people can actually use.

## Contact

[LinkedIn](https://www.linkedin.com/in/nathan-marinas-pose/) · [Email](mailto:nathanmarinaspose@gmail.com)
