## SciPy with a real historical dataset

This GitHub-ready folder accompanies the **36-slide Week 7 lesson**. The four
original SciPy topics are covered through **three connected investigations**:

1. **Integration:** accumulated CO₂ concentration anomaly.
2. **Interpolation and clustering:** reconstruct missing readings and group seasonal shapes.
3. **Linear systems and scientific imaging:** fit a model, then process a photograph
   and the same CO₂ data as a heatmap (Parts **3A** and **3B**).

All investigations use the **complete 2,284-row historical Mauna Loa dataset**;
the image activity also uses a supplied 512×512 grayscale image.

### Files

```text
week07-scipy/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── COM7024_Lesson7_MaunaLoa_CO2_Full.csv
│   └── COM7024_Lesson7_Camera_Practice_Image.png
└── notebooks/
    ├── 00_dataset_orientation.ipynb
    ├── 01_accumulated_co2_anomaly.ipynb
    ├── 02_interpolation_and_seasonal_clustering.ipynb
    ├── 03A_least_squares_co2_modelling.ipynb
    └── 03B_image_and_co2_heatmap.ipynb
```

### Getting started

1. Download this folder, or clone the course GitHub repository.
2. From `week07-scipy/`, install packages:
   ```bash
   python -m pip install -r requirements.txt
   ```
3. Start JupyterLab / Jupyter Notebook, or open the `.ipynb` files in VS Code.
4. Run `notebooks/00_dataset_orientation.ipynb` first.
5. Work through Activities 1, 2, 3A, and 3B. Each notebook has working examples,
   real-data calculations, independent questions, and an optional extension.

**Google Colab:** Upload a notebook **and the two data files**. Place the data
files in a `data/` folder, or in the same working directory as the notebook.
Colab resets uploaded files when its runtime is restarted.

### Activity guide

| Notebook | Main task | Suggested time | Expected output |
|---|---|---:|---|
| 00 · Orientation | Audit full data, check environment | 15–20 min | Summary and initial chart |
| 01 · Integration | Accumulated anomaly above 315 ppm | 30–40 min | Area in ppm·years and cumulative chart |
| 02 · Interpolation/clustering | Holdout validation and seasonal groups | 40–50 min | RMSE table, heatmap, clusters |
| 03A · Least squares | Compare trend and seasonal models | 30–40 min | Coefficients, RMSE, residuals |
| 03B · Image processing | Photo transforms and CO₂ heatmap | 25–35 min | Before/after visualisations |

The activities can be distributed across the teaching session or assigned as
follow-up independent work. For a shorter session, prioritise **01, 02 and 03A**;
03B is a practical extension to the third investigation.

### Learning outcomes

By the end of the lesson, students should be able to:
- Apply SciPy numerical methods to realistic data analytics problems.
- Prepare and analyse a full historical dataset using appropriate methods.
- Validate results, communicate uncertainty, and make evidence-based conclusions.

### Scientific cautions

- The CO₂ data are **historical** (1958–2001), not current measurements.
- The **315 ppm baseline is illustrative**, not an official threshold.
- Integrated concentration anomaly has units **ppm·years**, **not tonnes of CO₂ emissions**.
- Interpolated values are estimates; do not overwrite the raw series.
- Cluster membership describes similarity; it does not establish causation.
- Image smoothing changes values; report quantitative conclusions from the raw data.

### Reproducibility

- The data and practice image are supplied locally; no internet is required.
- Interpolation validation uses a fixed random seed (`7`).
- Every notebook is self-contained; there are no cross-notebook variables.
- Student notebooks include **working code plus independent tasks**, without
  the completed instructor-only extension answers.

### Data attribution

- **Weekly atmospheric CO₂ observations:** `statsmodels.datasets.co2`, Mauna Loa,
  as bundled in the course's Lesson 7 materials. See
  <https://www.statsmodels.org/stable/datasets/generated/co2.html>.
- **Grayscale camera image:** `skimage.data.camera`, distributed with
  scikit-image. See <https://scikit-image.org/docs/stable/api/skimage.data.html>.
- **Methods:** SciPy `integrate`, `interpolate`, `cluster.hierarchy`, `linalg`,
  and `ndimage`: <https://docs.scipy.org/doc/scipy/>.

