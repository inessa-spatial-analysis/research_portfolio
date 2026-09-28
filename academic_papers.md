[← Back to Home](index.md)


# Working Papers & Preprints

This section outlines my current academic research. My work bridges spatial econometrics, human mobility modeling, and machine learning to understand how the new norm of remote work reshapes urban ecosystems.

---

## 📄 Working Papers

### Working from Home and Urban Rental Markets: Evidence from the Tel Aviv Metropolitan Area
*Co-authored with Matan Gdaliahu* | [**View on ResearchGate**](https://www.researchgate.net/publication/395945061_Estimating_the_impact_of_working_from_home_on_urban_equilibrium_neighborhood_scale_effects_using_mobile_data)

**Abstract & Core Findings:** 
This paper investigates how the transition to hybrid work alters the spatial distribution of residential rental prices. By leveraging an Alonso-Muth-Mills monocentric-city framework, we demonstrate that a reduced commuting burden flattens the rent-distance gradient and amplifies the value of local consumption amenities. Using nearly four years of high-resolution GPS-signal data across 620 neighborhoods, we find compelling evidence of a "donut effect". WFH-capable households increasingly relocate to suburban, high-amenity neighborhoods. Consequently, a higher lagged neighborhood WFH rate depresses rents in areas closest to the Central Business District (CBD) while raising them in distant, high-amenity peripheries.

**Methodological Focus:**
*   **Data Engineering:** Processing massive datasets of raw mobile GPS signals to filter out noise, cluster geolocated 'stays', dynamically identify home and work anchors, and compute high-resolution neighborhood-level WFH rates and residential migration trajectories
*   **Econometrics:** Dynamic Two-Way Fixed Effects (TWFE) panel regressions with neighborhood and quarter fixed effects to isolate spatial rental pressures.

### Decoding Place Functionality: Identifying Emerging Third Places and the Drivers of Remote Work Visitation via Human Trajectories
*(Working Paper)* | [**slides**](https://github.com/inessa-spatial-analysis/research_portfolio/blob/main/ersa_2026_v2.pdf)

**Abstract & Core Findings:**
This research examines the role of "new third places" (e.g., cafes, libraries) within the 15-minute city concept in the post-COVID era, alongside their impact on the local economy through housing prices. Using mobile GPS trajectories in the Tel Aviv Metropolitan Area from 2022-2023, I mapped how these non-traditional workspaces function as office substitutes that shift daytime professional activity away from the CBD. Initial findings reveal a distinct new behavioral pattern at these venues, characterized by an increase in extended early-afternoon stays. Furthermore, the results demonstrate that the availability of third places effectively anchors residents, leading them to spend significantly more time in their local neighborhood outside of the home.

**Methodological Focus:**
*   **Spatial Machine Learning:** Implemented Positive-Unlabeled (PU) learning using an Elastic-Net Logistic Regression with Elkan-Noto probability adjustments to classify true third places using Google Reviews as positive ground truth.
*   **Trajectory Embeddings:** Utilized a Word2Vec skip-gram architecture to generate location embeddings from chronological human trajectories, measuring the semantic cosine distance of POIs to formal "work" locations.
*   **Econometrics:** Stepwise TWFE panel regression estimated via Weighted Least Squares (WLS).

### A Unified Framework for Tracking Working-From-Home Using Mobile Phone Data
*(Working Paper)* | [**GitHub**](https://www.researchgate.net/publication/395945061_Estimating_the_impact_of_working_from_home_on_urban_equilibrium_neighborhood_scale_effects_using_mobile_data)

**Abstract & Core Findings:**
This methodological paper develops a scalable, geography-independent approach to estimating granular WFH rates using passively collected GPS signals, overcoming the spatial biases and low resolution of traditional surveys. The framework relies on Bayesian conditional probability to account for non-uniform hourly signal sampling and individualized working schedules. The method was rigorously validated against the 2023 New Zealand Census data. 

**Methodological Focus:**
*   **Bias Correction:** Formulated an Inverse Probability Weighting (IPW) framework to correct for demographic sampling skew and spatial selection bias in the mobile data.
*   **Signal Isolation:** Applied an intermediate WLS regression to mathematically purge structural home-worker noise (e.g., agricultural workers) before validating the core telecommuting metric.
*   **Geospatial Processing:** Applied spatial smoothing techniques utilizing Geohash indices to mitigate GPS jitter and accurately anchor user home and work locations. 

---

## 🎓 Academic Theses

### Analysing relationships between museums and local economic activities by mobile phone data in Moscow
*MSc Urban Analytics, University of Glasgow* | [**Paper**] (https://github.com/inessa-spatial-analysis/research_portfolio/blob/main/thesis_final_20.01.pdf)

**Abstract:**
This thesis explores the localized economic impact of museums by analyzing their capacity to attract affluent and young pedestrians to surrounding neighborhoods[cite: 5]. The study leverages high-resolution mobile phone app data in Moscow, applying Geographically Weighted Regressions (GWR) to control for built-environment features such as walkability and street connectivity[cite: 5]. The findings reject the assumption of a universal culture-led economic regeneration, demonstrating instead that museums successfully drive local economic activity only in specific residential contexts where they function as interactive community hubs[cite: 5].
