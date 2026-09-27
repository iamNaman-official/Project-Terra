# 🌍 Project Terra

> **NASA Space Apps Challenge 2026 — Earth System Trend Detective**

Project Terra is a collaborative **learning, experimentation, and development laboratory** for investigating changes in Earth's systems using NASA Earth-observation data.

The repository is designed to let the team learn, experiment, test hypotheses, analyze data, document discoveries, and gradually turn validated ideas into reusable software and eventually a complete application.

---

## 🎯 Mission

Earth is a dynamic system.

Land, vegetation, temperature, water, atmosphere, and other components change over time and space.

Project Terra aims to investigate these changes using scientific data and computational methods.

The core questions we want to answer are:

* **What is changing?**
* **Where is it changing?**
* **How much is it changing?**
* **How has it changed over time?**
* **Is the observed change statistically significant?**
* **Can unusual patterns or anomalies be detected?**
* **How can these findings be communicated clearly?**

---

## 🛰️ Challenge

**NASA Space Apps Challenge 2026**

**Challenge:** Earth System Trend Detective

The project will explore NASA Earth-observation datasets to identify, analyze, and communicate meaningful spatial and temporal trends in Earth's systems.

Our approach combines:

* NASA Earth-observation data
* Data engineering
* Statistics
* Trend analysis
* Statistical significance testing
* Machine learning
* GIS and spatial analysis
* Data visualization
* Backend engineering
* Frontend development

---

# 🧪 Project Philosophy

Terra is **not being built as a production application from day one**.

It is a laboratory.

We want to learn the underlying concepts before turning them into application code.

Our general workflow is:

```text
Learn
  ↓
Experiment
  ↓
Test
  ↓
Validate
  ↓
Document
  ↓
Refactor
  ↓
Reusable Code
  ↓
Backend / API
  ↓
Frontend
  ↓
Terra Application
```

This means unfinished experiments are expected.

A notebook does not have to become production code.

An experiment can fail.

A statistical method can turn out to be unsuitable.

A model can perform poorly.

These are valuable results as long as we understand and document what happened.

---

# 🗂️ Repository Structure

```text
Project-Terra/
│
├── api-tests/          # API testing and Bruno collections
│
├── backend/            # Django backend and APIs
│
├── data/               # Local scientific datasets
│   ├── raw/
│   ├── processed/
│   └── samples/
│
├── docs/               # Project knowledge and documentation
│   ├── architecture/
│   ├── datasets/
│   ├── experiments/
│   ├── learning/
│   └── notes/
│
├── experiments/        # Experimental and exploratory code
│   ├── data/
│   ├── statistics/
│   ├── ml/
│   ├── gis/
│   └── remote_sensing/
│
├── frontend/            # React frontend
│
├── notebooks/           # Jupyter exploration and analysis
│   ├── data_exploration/
│   ├── statistics/
│   ├── ml/
│   ├── gis/
│   └── remote_sensing/
│
├── scripts/             # Utility and automation scripts
│
├── src/                 # Reusable validated code
│   ├── data/
│   ├── analysis/
│   ├── ml/
│   ├── gis/
│   └── visualization/
│
└── tests/               # Tests for reusable code
```

---

# 🔬 Experiments vs Reusable Code

One of the most important conventions in Terra is the distinction between **experimentation** and **reusable software**.

### `experiments/`

Use this when you are:

* Trying an idea
* Testing a method
* Learning a library
* Comparing algorithms
* Exploring a dataset
* Writing temporary code
* Investigating a hypothesis

Experimental code does not need to be perfectly structured.

### `src/`

Use this when the code has been:

* Tested
* Validated
* Understood
* Documented
* Refactored
* Found useful beyond one experiment

For example:

```text
experiments/statistics/
        │
        │  experiment
        ▼
   validate method
        │
        ▼
src/analysis/trends/
        │
        ▼
      tests/
```

---

# 🛰️ Initial Scientific Direction

Our first dataset is planned to be:

**MODIS/Terra Land Surface Temperature/Emissivity 8-Day L3 Global 1 km V061 — MOD11A2.061**

The initial goal is not immediately to build an ML model.

First, we want to understand the data.

### Initial investigation

```text
NASA Dataset
     ↓
Understand variables
     ↓
Understand dimensions
     ↓
Understand units
     ↓
Understand quality flags
     ↓
Select a small region
     ↓
Clean / validate data
     ↓
Create time series
     ↓
Calculate trends
     ↓
Test statistical significance
     ↓
Create spatial trend maps
     ↓
Investigate anomalies
```

Machine learning can then be explored as an additional method rather than replacing scientific statistical analysis.

---

# 🧰 Technology Areas

## Data & Scientific Computing

* Python
* NumPy
* pandas
* xarray
* NetCDF
* HDF5
* SciPy
* statsmodels
* PyMannKendall

## Statistics

* Descriptive statistics
* Time-series analysis
* Trend analysis
* Mann-Kendall testing
* Statistical significance
* Regression
* Uncertainty analysis

## Machine Learning

* scikit-learn
* Feature engineering
* Clustering
* Anomaly detection
* Dimensionality reduction

## GIS & Remote Sensing

* QGIS
* GeoPandas
* Rasterio
* rioxarray
* Shapely
* PyProj

## Backend

* Python
* Django
* Django REST Framework
* PostgreSQL
* PostGIS

## Frontend

* React
* TypeScript
* Vite
* Tailwind CSS
* Leaflet
* Plotly

## Development & Collaboration

* Git
* GitHub
* GitHub Actions
* JupyterLab
* VS Code
* PyCharm
* Bruno
* pytest
* Ruff

---

# 👥 Team Roles

Project Terra is divided into six primary areas.

| Role  | Area                          | Main Responsibility                                     |
| ----- | ----------------------------- | ------------------------------------------------------- |
| 🛰️ 1 | NASA Data + Earth Science     | Understand NASA datasets and scientific context         |
| 📊 2  | Statistics + Data Engineering | Process data and perform statistical analysis           |
| 🤖 3  | AI/ML                         | Explore machine learning and anomaly detection          |
| 🌎 4  | GIS + Visualization           | Spatial analysis, maps, and geospatial visualization    |
| 🎨 5  | Frontend + UX                 | Build the user-facing interface and visual experience   |
| ⚙️ 6  | Backend + DevOps              | APIs, backend services, infrastructure, and integration |

These roles are areas of responsibility, not isolated silos.

Team members are encouraged to learn outside their assigned area.

---

# 📚 Learning First

Terra is also a learning repository.

If you learn something important, document it.

Examples:

```text
docs/learning/
```

can contain:

* Remote sensing concepts
* Statistical concepts
* GIS concepts
* Machine learning concepts
* Data formats
* NASA data processing notes
* Backend concepts
* Frontend concepts

The objective is to make knowledge reusable by the entire team.

---

# 📊 Data Policy

Large scientific datasets should **not** be committed to Git.

Use:

```text
data/raw/
```

for downloaded raw datasets.

Use:

```text
data/processed/
```

for locally processed datasets.

Use:

```text
data/samples/
```

for small datasets that are useful for reproducible experiments.

Dataset information should be documented in:

```text
docs/datasets/
```

Each important dataset should have information about:

* Source
* Dataset version
* Variables
* Units
* Spatial resolution
* Temporal resolution
* Quality flags
* Processing steps
* Known limitations

---

# 🧪 Experiments

Experiments should answer a question.

A useful experiment should document:

```text
Question
   ↓
Hypothesis
   ↓
Method
   ↓
Data
   ↓
Experiment
   ↓
Result
   ↓
Interpretation
   ↓
Limitations
   ↓
Next Step
```

An experiment that disproves an idea is still useful.

---

# 🧪 Testing

Testing is not limited to web application code.

We also want to verify scientific computations.

Examples:

* Does a temperature conversion produce the expected values?
* Does a trend calculation behave correctly?
* Are invalid pixels removed correctly?
* Are quality flags interpreted correctly?
* Does a spatial transformation preserve coordinates?
* Does an API return the expected response?
* Does an anomaly detector behave correctly on known sample data?

Scientific results should be reproducible wherever practical.

---

# 🌐 Backend & Frontend

The backend and frontend will be developed after we have validated useful scientific workflows.

The intended direction is:

```text
NASA Data
    ↓
Data Processing
    ↓
Scientific Analysis
    ↓
Validated Reusable Code
    ↓
Backend API
    ↓
Frontend
    ↓
User
```

The frontend should not be responsible for processing massive raw NASA datasets.

The backend should expose useful processed information and analysis results.

---

# 🔌 API Testing

API requests will be maintained under:

```text
api-tests/bruno/
```

Using Bruno allows API requests to be:

* Version controlled
* Shared
* Reproduced locally
* Reviewed alongside code

---

# 💻 Development Philosophy

We prefer understanding over blindly copying.

When using AI tools, generated code should be:

1. Read
2. Understood
3. Tested
4. Modified when necessary
5. Documented when important

AI can accelerate experimentation, but the team should understand the systems being built.

---

# 🌐 Offline-First Experiments

Once datasets and dependencies are available locally, scientific experiments should be able to run without requiring continuous internet access.

Internet access is primarily needed for:

* Downloading NASA datasets
* Documentation
* Dependency installation and updates
* GitHub collaboration
* External APIs
* Deployment

Local datasets and experiments should remain usable offline whenever practical.

---

# 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/iamNaman-official/Project-Terra.git
cd Project-Terra
```

Then explore:

```text
experiments/
notebooks/
docs/
data/
src/
```

The project application itself will be developed progressively.

Do not expect every directory to contain code immediately.

---

# 🤝 Contributing

Before starting work:

1. Understand the area you are working in.
2. Check existing experiments and documentation.
3. Create a branch for your work.
4. Experiment locally.
5. Document important findings.
6. Add tests where appropriate.
7. Open a pull request.

See:

```text
CONTRIBUTING.md
```

for the contribution workflow.

---

# 🌱 Current Status

Project Terra is currently in the:

> **Learning → Experimentation → Validation**

stage.

The immediate priority is to understand the scientific data and establish reliable analysis workflows before building the final application.

---

# 🗺️ Long-Term Direction

```text
NASA Earth Data
       ↓
Data Understanding
       ↓
Data Engineering
       ↓
Statistical Analysis
       ↓
Trend Detection
       ↓
Significance Testing
       ↓
ML / Anomaly Detection
       ↓
GIS Analysis
       ↓
Visualization
       ↓
Backend APIs
       ↓
Frontend
       ↓
Project Terra
```

The final system should help users explore meaningful changes in Earth's systems and understand the evidence behind those changes.

---

## 🌍 Build. Experiment. Understand. Discover.

**Project Terra — NASA Space Apps Challenge 2026**
