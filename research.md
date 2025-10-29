---
layout: sidebar
title: Research & Projects
---

# Research & Projects

My research focuses on the intersection of computational chemistry, data science, and pharmaceutical development. Below are my key research areas:

---

## 🧬 Molecular Dynamics Simulations {#md-simulations}

### Overview
Specialized in computational simulations of protein systems, particularly antibodies, to understand molecular interactions and stability mechanisms critical for drug formulation.

### Key Projects

#### Protein-Cosolute Interactions Studies
**Objective:** Investigate how cosolutes (urea, arginine, salts) affect antibody structure and stability

**Methodology:**
- All-atom molecular dynamics simulations using GROMACS, NAMD, OpenMM
- Multi-microsecond timescale simulations on HPC clusters
- Analysis using MDAnalysis, custom Python scripts
- Kirkwood-Buff theory for thermodynamic interpretation

**Key Findings:**
- Discovered domain-specific binding preferences of urea to antibodies
- Identified multiple destabilization pathways affecting therapeutic proteins
- Developed expression for diffusion interaction parameters

**Publications:**
1. "Multidomain Protein−Urea Interactions: Differences in Binding Behavior Lead to Different Destabilization Tendencies for Monoclonal Antibodies" - J. Phys. Chem. B (2024)
2. "Impact of Urea on Monoclonal Antibodies: Multiple Destabilization and Aggregation Effects" - ACS Omega (2024)
3. "An Expression for the Diffusion Interaction Parameter for Pharmaceutical Formulations" - Phys. Chem. Chem. Phys. (2025)

#### Antibody Stress Testing and Stability
**Objective:** Develop computational protocols for predicting antibody stability under stress conditions

**Approach:**
- Forced degradation simulations (thermal, chemical stress)
- Enzymatic digestion modeling
- Aggregation propensity prediction
- Conformational multi-state analysis

**Impact:** Enhanced understanding of antibody behavior during manufacturing and storage

#### Small-Molecule Drug Research
**Focus:** Chemical sequence variants and their effects on drug properties

**Tools & Software:**
- GROMACS for biomolecular simulations
- NAMD for large-scale MD simulations
- OpenMM for custom force field development
- VMD for visualization and trajectory analysis

**Computational Resources:**
- Linux HPC clusters with Slurm batch system
- Bash scripting for workflow automation
- Parallel computing for production simulations

### Under Review
"Computational Simulations of Antibodies in Solution: Study of Physicochemical Properties and Interactions with Co-Solutes" - Applied Physics Review (Invited Review)

---

## 📊 Advanced Spectroscopic Data Analysis {#spectroscopy}

### Overview
Development of machine learning approaches for automated analysis of spectroscopic data in protein characterization and formulation development.

### Key Projects

#### ML-Powered Spectral Deconvolution
**Challenge:** Traditional spectroscopic analysis requires manual interpretation and is time-intensive

**Solution:**
- Developed machine learning models for automated spectral pattern recognition
- Created algorithms for deconvolution of overlapping spectroscopic signals
- Implemented feature extraction for antibody and excipient characterization

**Techniques:**
- Supervised learning (scikit-learn, PyTorch)
- Dimensionality reduction (PCA, t-SNE)
- Pattern recognition algorithms
- Ensemble methods for robust predictions

**Results:**
- 95%+ accuracy in antibody classification
- 10x faster analysis compared to manual methods
- Scalable to high-throughput screening

#### Automated Liquid Handling Workflows
**Objective:** Design end-to-end automation for protein characterization studies

**Implementation:**
- Python-based control of liquid handling robots
- Real-time data acquisition and processing
- Integration with spectroscopic instruments
- Automated quality control and flagging

**Technologies:**
- Python (pandas, numpy, matplotlib)
- Custom APIs for instrument control
- Database integration for sample tracking
- Streamlit dashboards for data visualization

**Impact:** Reduced manual workload by 80%, increased experimental reproducibility

#### Protein Characterization Techniques

**Spectroscopy Methods:**
- **UV/Vis Spectroscopy** - Protein concentration, stability
- **Circular Dichroism (CD)** - Secondary structure analysis
- **Infrared (IR) Spectroscopy** - Tertiary structure, aggregation
- **Fluorescence Spectroscopy** - Environmental sensitivity, unfolding

**Calorimetry & Light Scattering:**
- **Differential Scanning Calorimetry (DSC)** - Thermal stability
- **nanoDSF** - High-throughput thermal unfolding
- **Dynamic Light Scattering (DLS)** - Aggregation, size distribution

**Chromatography:**
- **UPLC-CAD** - Surfactant analysis in formulations
- Method development for excipient profiling

### Tools & Software
- Python (scikit-learn, PyTorch, RDKit, MDAnalysis)
- SIMCA for multivariate analysis
- Spotfire for industrial analytics
- Excel VBA for legacy system integration

---

## 🔬 Data Science in Drug Development {#drug-development}

### Overview
Application of machine learning and statistical methods to pharmaceutical research, from formulation optimization to molecular property prediction.

### Key Projects

#### Surfactant Degradation Profiling (Master's Thesis)
**Problem:** Surfactants in drug formulations degrade over time, affecting drug stability

**Approach:**
- Developed ML model for pattern recognition of degradation profiles
- Enabled classification and clustering of degraded lipid chains
- Used UPLC-CAD data for training and validation

**Methodology:**
- Time-series analysis of chromatographic data
- Unsupervised clustering for degradation pattern identification
- Supervised classification for stability prediction

**Outcome:** 
- Early detection of formulation instability
- Rational selection of surfactants for long-term stability

#### Solvation Energy Prediction Neural Networks
**Objective:** Predict solvation energies of electrolytes from molecular structure

**Innovation:**
- Combined conceptual Density Functional Theory (DFT) with neural networks
- Used atomistic properties as input features
- Validated on experimental and computational datasets

**Publications:**
- "Artificial neural networks for the prediction of solvation energies based on experimental and computational data" - Phys. Chem. Chem. Phys. (2020)
- "Combination of Explainable Machine Learning and Conceptual Density Functional Theory" - Phys. Chem. Chem. Phys. (2022)

**Impact:** Accelerated screening of formulation components

#### Explainable AI for Drug Discovery
**Focus:** Interpretable machine learning for understanding structure-property relationships

**Methods:**
- SHAP values for feature importance
- Attention mechanisms in neural networks
- Conceptual DFT descriptors
- Chemical interpretability

**Applications:**
- Formulation excipient selection
- Drug-protein interaction prediction
- Stability assessment

### Technical Skills
- **Python Libraries:** PyTorch, scikit-learn, RDKit, pandas, numpy
- **R:** Statistical analysis, visualization
- **SQL:** Database queries for large datasets
- **HPC:** Bash scripting, Slurm batch systems
- **Cloud Platforms:** Databricks, Streamlit for deployment

---

## 📈 Data Science in Patent & Clinical Analytics {#patent-analytics}

### Overview
Application of AI and data science methodologies to patent analytics and clinical research, supporting strategic decision-making in pharmaceutical R&D.

### Patent Analytics Project

#### AI and Data Science for Global Patent Search & Analytics
**Organization:** Boehringer Ingelheim, Global Data Science Team  
**Duration:** January 2024 - February 2024

**Project Scope:**
- Developed AI-driven patent search and analysis tools
- Implemented natural language processing for patent document analysis
- Created competitive intelligence dashboards
- Designed predictive models for patent landscape trends

**Technologies:**
- **NLP:** Text mining, entity recognition, document classification
- **Machine Learning:** Clustering algorithms for patent families
- **Visualization:** Interactive dashboards for strategic insights
- **Databases:** Patent database integration and querying

**Deliverables:**
- Automated patent search pipeline
- Competitive analysis framework
- Trend identification algorithms
- Strategic recommendations for IP portfolio

**Business Impact:**
- Accelerated prior art search process
- Identified white space opportunities
- Enhanced freedom-to-operate analysis

### Clinical Data Science

#### BI OPEN Global Data Science Challenge
**Award:** Engagement Individual Award (June 2021)  
**Project:** Lung Acoustic Signal Detection

**Challenge:**
- Analyze respiratory acoustic signals for disease detection
- Develop ML models for classification of lung conditions
- Work with complex biomedical time-series data

**Approach:**
- Signal processing and feature extraction
- Deep learning for acoustic pattern recognition
- Cross-validation strategies for medical data
- Model interpretability for clinical acceptance

**Skills Demonstrated:**
- Biomedical signal processing
- Time-series analysis
- Healthcare data privacy and ethics
- Model validation for clinical applications

### Methodologies

**Data Analytics:**
- Exploratory data analysis (EDA)
- Statistical hypothesis testing
- Regression and classification models
- Time-series forecasting

**Text Mining & NLP:**
- Document similarity and clustering
- Named entity recognition
- Sentiment analysis
- Topic modeling

**Visualization & Reporting:**
- Interactive dashboards (Streamlit, Plotly)
- Statistical graphics (matplotlib, seaborn)
- Business intelligence tools (Spotfire)
- Automated reporting pipelines

### Industry Applications

**Patent Intelligence:**
- Competitive landscape analysis
- Technology trend forecasting
- IP portfolio optimization
- Freedom-to-operate assessments

**Clinical Research:**
- Biomarker discovery
- Patient stratification
- Treatment outcome prediction
- Real-world evidence analysis

---

## 🛠️ Technical Infrastructure

### Programming & Tools
- **Languages:** Python, R, SQL
- **ML Frameworks:** PyTorch, scikit-learn, TensorFlow
- **Cheminformatics:** RDKit, Open Babel
- **MD Analysis:** MDAnalysis, PyMOL, VMD
- **Data Science:** pandas, numpy, scipy
- **Visualization:** matplotlib, seaborn, Plotly

### High-Performance Computing
- Linux HPC clusters
- Slurm batch scheduling
- Parallel computing (MPI, OpenMP)
- Bash scripting for automation

### Cloud & Collaboration
- Databricks for distributed computing
- Streamlit for web applications
- Git/Bitbucket for version control
- Jupyter notebooks for reproducible research

---

[View Publications →](/publications) | [Explore Skills →](/skills) | [Contact Me →](/contact)
