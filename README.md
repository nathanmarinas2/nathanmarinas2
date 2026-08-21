# Nathan Mariñas Pose

**AI Engineer** focused on applied machine learning, AI systems and data-intensive products.

BSc in Artificial Intelligence — **Universidade da Coruña (2022–2026)**. Previously **AI Engineer Intern at ABANCA**, working on GenAI, RAG reliability and forecasting (**9.2/10 final review**).

📰 **Featured in [El Español / Quincemil](https://www.elespanol.com/quincemil/a-coruna/20260223/proyecto-estudiante-usc-busca-revolucionar-bicicoruna-falla-tiempo/1003744139453_0.html)** for my independent ML and data analysis of A Coruña's BiciCoruña bike-sharing network.

I work on AI systems beyond the model itself: where the data comes from, how outputs are evaluated and validated, what the system is allowed to touch, and what happens when it is uncertain or wrong.

**Models are components. Reliable systems are the product.**

📍 A Coruña, Spain · [LinkedIn](https://www.linkedin.com/in/nathan-marinas-pose/) · [Email](mailto:nathanmarinaspose@gmail.com)

---

## Selected Work

### 🚲 [BiciCoruña Fleet Optimization](https://github.com/nathanmarinas2/bicicoruna-fleet-optimization)

**Real-time Data Engineering · Machine Learning · Urban Mobility**

Independent technical analysis of A Coruña's public bike-sharing network, from building the historical dataset to predictive modeling and operational recommendations.

There was no consolidated public historical dataset for the service, so **I built it from scratch**.

* Built and deployed a Node.js collector polling the GBFS feed of **all 79 stations every 5 minutes**
* Developed a **LightGBM stockout classifier** with a 30-minute prediction horizon
* Achieved **F1 = 0.78** and **87% accuracy**
* Tuned the operational stockout threshold to provide useful reaction time before complete unavailability
* Segmented stations into **4 behavioral archetypes** using K-Means
* Quantified spatial and temporal service failures across the network
* Tested transfer learning from approximately **500k Barcelona Bicing records**; it produced no meaningful improvement over the local model, so I discarded the additional complexity and documented the negative result
* Converted the analysis into concrete fleet-rebalancing and capacity recommendations

The project demonstrates the complete chain:

**data collection → feature engineering → experimentation → evaluation → operational decision**

`Python` · `LightGBM` · `Pandas` · `Node.js` · `Streamlit` · `Leaflet` · `Railway`

**→ [Repository](https://github.com/nathanmarinas2/bicicoruna-fleet-optimization)**


---

### 🎵 [Music Graph Explorer](https://github.com/nathanmarinas2/music-graph-explorer)

**Graph ML · Representation learning · Browser-side inference**

A large-scale music intelligence system for exploring artist relationships through collaboration graphs and learned embeddings.

The embeddings were not the hard part. **Shipping them was.**

* Built a public collaboration graph containing **100,000 artists and 1,059,326 edges**
* Constructed and processed the graph using **DuckDB**
* Trained **64-dimensional Node2Vec-style embeddings** from graph random walks
* Projected the latent space into 3D with **UMAP**
* Built interactive exploration with **Three.js**
* Added shortest-path discovery between artists with track-aware route explanations
* Quantized embeddings from float32 to int8 for client-side inference
* Compressed the public embedding bundle to approximately **6.1 MB**
* Implemented **MixDNA lite** directly in the browser
* Shipped the complete experience as a static site with **no backend dependency**

The engineering question became:

> How do you turn a large offline ML pipeline into something users can open in a browser and use immediately?

`Python` · `DuckDB` · `Gensim` · `UMAP` · `JavaScript` · `Three.js`

**→ [Live Demo](https://nathanmarinas2.github.io/music-graph-explorer/) · [Repository](https://github.com/nathanmarinas2/music-graph-explorer)**

---

### ⚡ [EnergiaPredictorES](https://github.com/nathanmarinas2/EnergiaPredictorES)

**Time-series forecasting · ML experimentation · Model selection**

Electricity-demand forecasting system for Spain comparing classical machine learning, deep learning and statistical baselines.

* Built preprocessing and feature-engineering pipelines for temporal data
* Engineered cyclical time features, lag variables, rolling statistics and calendar information
* Compared **LightGBM, XGBoost, Temporal Fusion Transformer and statistical baselines**
* Best model: **LightGBM — 1.15% MAPE**
* XGBoost: **1.46% MAPE**
* Seasonal-naive baseline: approximately **9.5% MAPE**
* Analyzed why the more complex deep-learning experiment underperformed instead of hiding the result
* Structured the project as a reproducible pipeline with separate data, model and evaluation components

The conclusion I care about:

**Model complexity has to earn its place.**

A simpler model with the right representation of the problem can be substantially more useful than a more sophisticated architecture deployed for its own sake.

`Python` · `LightGBM` · `XGBoost` · `PyTorch` · `Darts` · `Pandas`

**→ [Repository](https://github.com/nathanmarinas2/EnergiaPredictorES)**

---

### 🌪️ [Green Energy Sentinel](https://github.com/nathanmarinas2/Green-Energy-Sentinel)

**Geospatial analytics · Decision systems · Renewable energy**

Multi-criteria decision-support system for identifying suitable wind-farm locations in Galicia while accounting for environmental risk.

* Integrated **Global Wind Atlas** raster data at 100 m height
* Processed **40,000+ historical lightning observations** from MeteoGalicia
* Converted discrete lightning events into a continuous spatial-risk surface using Gaussian KDE
* Applied geographic land masks using GeoJSON administrative boundaries
* Combined wind-resource potential and lightning risk into a suitability model
* Validated high-suitability regions against existing wind-turbine locations retrieved through the OpenStreetMap Overpass API
* Built interactive 2D, 3D and temporal geospatial visualizations

This project sits at the intersection of **data engineering, geospatial analysis and decision modeling** rather than conventional supervised ML.

`Python` · `Rasterio` · `GeoJSON` · `Folium` · `PyDeck` · `GIS`

**→ [Repository](https://github.com/nathanmarinas2/Green-Energy-Sentinel)**

---

### 🚌 BUS-CO

**Product engineering · Urban mobility · Edge-first web architecture**

Real-time public transport Progressive Web App built for A Coruña.

I designed and developed the product end-to-end, from transport-data integration and routing logic to the mobile interface and deployment architecture.

* Built a mobile-first **PWA with Vanilla JavaScript**
* Integrated public-transport data, geolocation and interactive maps
* Used local caching and Cloudflare infrastructure for near-instant route searches
* Designed a privacy-first architecture with client-side processing
* Avoided third-party advertising and tracking dependencies
* Built for fast loading and usability on mobile connections

BUS-CO is useful to me as a portfolio project for a different reason than the ML work: it demonstrates that I can take a technical idea all the way to a **user-facing product**.

`JavaScript` · `Cloudflare` · `Leaflet` · `HTML` · `CSS` · `Git`

---

## Research

### 🔭 Deep Learning on Gaia & Euclid astronomical data

Academic research involving machine-learning methods applied to astronomical data from the **Gaia and Euclid missions**.

The work focuses on the characterization of stellar systems and the search for substellar companions using spectroscopic and photometric information.

It involves:

* Large-scale scientific data processing
* Feature engineering
* Classification and representation problems
* Neural-network experimentation
* Model evaluation
* Astronomical catalog cross-matching
* Analysis of model limitations and scientific uncertainty

Research carried out in the context of **CITIC / LIA2** and my BSc final project.

---

## Experience

### 🏦 AI Engineer Intern — ABANCA

**Business Process Optimization · 2025**

Worked on GenAI and predictive systems inside a banking environment.

**Final performance review: 9.2/10**

#### RAG & LLM systems

* Designed a **RAG-Readiness framework** to evaluate internal documentation before LLM ingestion
* Built logic to identify documentation issues that could degrade retrieval quality
* Worked on context-management strategies for customer-support tooling
* Reduced hallucination rates by approximately **40% in long-context sessions**
* Worked with Gemini-based systems under strict privacy constraints

A major lesson from the work was that many apparent "LLM problems" are actually **data, context or system-design problems**.

#### Forecasting

* Developed a **LightGBM demand-prediction model** for service-volume forecasting
* Designed validation logic that checks whether the available data supports ML inference
* Added fallback behavior to statistical baselines when the predictive signal is insufficient

Rather than always forcing an ML prediction, the system could degrade to something simpler and more defensible.

#### Security

All work was performed inside self-contained environments under banking security and data-privacy requirements.

`Python` · `LightGBM` · `LLMs` · `RAG` · `Data Analysis`

---

### 🧩 Founder — NAMASE

[**namase.es**](https://namase.es)

Technology studio focused on applying software, automation and AI to concrete business processes.

My work includes:

* Understanding how information moves through a business
* Identifying repetitive or failure-prone processes
* Connecting previously isolated systems
* Designing workflow automations and internal tools
* Defining which cases can be automated and which require human review
* Building AI-enabled systems with explicit validation and fallback paths
* Developing web products and commercial infrastructure

The principle behind the work is simple:

**Automation should reduce operational complexity, not hide it behind another layer of software.**

---

## Education

### 🎓 Universidade da Coruña

**BSc in Artificial Intelligence**
2022–2026

The degree covered the full stack behind intelligent systems rather than ML in isolation.

Core areas included:

* Machine Learning
* Advanced Machine Learning
* Deep Learning
* Natural Language Processing
* Information Retrieval & Web Mining
* Computer Vision
* Knowledge Representation & Reasoning
* Multi-Agent Systems
* Mathematical Optimization
* Algorithms & Data Structures
* Databases
* Software Engineering
* Concurrent, Parallel & Distributed Computing
* Data Processing & Analysis
* AI Systems Development & Deployment
* Cybersecurity
* AI Law, Security & Ethics

---

## Tech

| Area                 | Technologies                                                  |
| -------------------- | ------------------------------------------------------------- |
| **Machine Learning** | Python, Scikit-learn, LightGBM, XGBoost                       |
| **Deep Learning**    | PyTorch, TensorFlow                                           |
| **Data**             | Pandas, NumPy, DuckDB, SQL                                    |
| **LLM Systems**      | RAG, context management, evaluation, prompt/output validation |
| **Time Series**      | Feature engineering, forecasting, Darts                       |
| **Computer Vision**  | OpenCV                                                        |
| **Geospatial**       | Rasterio, Folium, PyDeck, GeoJSON                             |
| **Web & Product**    | JavaScript, HTML/CSS, Leaflet, Three.js, Streamlit            |
| **Infrastructure**   | Docker, Cloudflare, Railway, Linux                            |
| **Tools**            | Git, GitHub Actions, Jupyter, VS Code                         |

---

## How I Work

**Start with the baseline.**
I want to know how much value the sophisticated approach actually adds.

**Complexity has to justify itself.**
A more advanced model is not automatically a better system.

**Negative results belong in the project.**
If an experiment does not work, understanding why is part of the result.

**Evaluation comes before confidence.**
A system should know when the available evidence is insufficient to trust its own output.

**Failure paths are part of the architecture.**
I care about what happens when a model is wrong, an input changes or an external dependency fails.

**The final artifact should be usable.**
I prefer systems people can open, test and understand over notebooks that only work in the author's environment.

---

## What I'm Interested In

I'm particularly interested in problems involving:

* **AI Engineering**
* **Machine Learning Engineering**
* Applied Machine Learning
* LLM & RAG systems
* Data-intensive products
* Forecasting
* ML evaluation and reliability
* Data pipelines
* Intelligent decision-support systems

Especially when the challenge is not simply training a model, but **making the complete system reliable and useful**.

---

## Contact

📍 **A Coruña, Spain**

[**LinkedIn**](https://www.linkedin.com/in/nathan-marinas-pose/) · [**Email**](mailto:nathanmarinaspose@gmail.com)

**Open to AI Engineering, Machine Learning Engineering and applied ML opportunities.**
