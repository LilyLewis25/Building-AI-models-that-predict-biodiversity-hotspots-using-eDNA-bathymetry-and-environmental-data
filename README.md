# Building-AI-models-that-predict-biodiversity-hotspots-using-eDNA-bathymetry-and-environmental-data
Environmental DNA (eDNA), ROV imagery, and oceanographic sensors offer new ways to link physical features to living communities. The challenge is integrating these multimodal data streams into a unified framework that can predict biodiversity in unexplored areas.

# 🌊 Predicting Marine Biodiversity with Multimodal Data  

**From structure to species: Building predictive AI models that fuse eDNA, bathymetry, imagery, and sensor data to identify unseen biodiversity hotspots.**

---

## 📌 Background  
OceanX has transformed our ability to collect high-resolution data on the ocean using ROVs, submersibles, mapping systems, and eDNA sampling. These efforts provide powerful raw data streams, but biodiversity monitoring often remains **site-specific and descriptive**.  

Our project pushes this further by creating a **predictive framework**: instead of only describing where biodiversity has been observed, we aim to **forecast where biodiversity is likely to occur** in unexplored areas. This helps bridge the gap between data-rich and data-poor regions of the ocean.  

---

## 🎯 Objectives  
- **Data fusion**: Combine structural (bathymetry), biological (eDNA), visual (ROV video), and physical (sensor) data into one integrated dataset.  
- **Predictive modelling**: Use machine learning to predict coral and sponge biodiversity in unsurveyed areas of Nola Seamount.  
- **Scalability**: Design a workflow that can be adapted to new sites and ecosystems (coral reefs, seagrass, mangroves, other seamounts).  
- **Decision support**: Produce biodiversity probability maps that can guide conservation, restoration, and exploration priorities.  

---

## 🛠 Technical Approach  

### 1. Data Integration  
- Align datasets spatially and temporally (bathymetry, eDNA sampling points, ROV tracks, sensor measurements).  
- Derive structural metrics from bathymetry (rugosity, slope, depth gradients).  
- Extract biodiversity “ground truth” from eDNA and annotated ROV imagery.  

### 2. Feature Engineering  
- Combine environmental drivers (temperature, salinity, oxygen, nutrients) with habitat features.  
- Encode eDNA richness as biodiversity indices (species presence/absence, richness scores).  
- Develop probabilistic features that account for current-driven eDNA drift.  

### 3. Machine Learning Modelling  
- Train supervised models (e.g., Random Forest, Gradient Boosting, CNN for imagery) using known biodiversity data.  
- Validate predictions against “hidden” biodiversity detections provided by OceanX.  
- Output probabilistic biodiversity maps with confidence scores.  

### 4. Visualisation  
- Interactive maps/dashboard of predicted hotspots.  
- Confidence layers to communicate uncertainty to scientists, managers, and decision-makers.  

---

## ⚠️ Uncertainty Handling  
Unlike standard biodiversity maps, our framework explicitly incorporates uncertainty:  

- **Currents & drift**: Oceanographic data (currents, salinity, stratification) help interpret whether eDNA detections are local or advected.  
- **Replication filters**: Consistent eDNA detections across multiple depths/locations weighted higher.  
- **Cross-validation**: Predictions checked against ROV detections.  
- **Confidence scores**: Maps highlight not only predicted biodiversity but also where predictions are strongest vs weakest.  

---

## 📊 Expected Outcomes  
- Predictive biodiversity map of unexplored Nola Seamount regions.  
- Generalised pipeline for multimodal biodiversity prediction.  
- Example use case: improving coral reef restoration planning by identifying future biodiversity hotspots, not just current ones.  
- Foundation for a **scalable, global monitoring framework** that extends OceanX’s exploratory data into **predictive biodiversity science**.  

---

## 🌍 Why This Project is Significant  
- **Goes beyond mapping**: OceanX already maps; we turn maps into predictions.  
- **Links structure to species**: Seafloor features + DNA + environment integrated for the first time in this challenge.  
- **Bridges shallow and deep ecosystems**: From coral reef restoration sites (Bali prototype) to deep seamounts.  
- **Supports decision-making**: Identifies not just what exists, but where to look next.  
- **Adds robustness**: Explicit handling of uncertainty makes outputs more scientifically credible.  

---

## 👩‍🔬 Team Roles  
- **Ecology & biodiversity**: Interpret drivers of biodiversity patterns.  
- **Data science**: Coding, machine learning, feature integration.  
- **Visualisation & communication**: Map design, dashboard creation, storytelling.  

---

## 📂 Repository Structure  

