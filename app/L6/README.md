# COM7024 · Week 6: pandas for Data Analytics

Student-facing Jupyter notebooks aligned with the **COM7024 Lesson 6 pandas teaching slides**. The notebooks are designed for classroom demonstrations, independent practice and upload to the course GitHub repository.

## Learning outcomes

By the end of the week, you should be able to:

1. Create and manipulate pandas Series and DataFrames.
2. Explore and transform datasets using indexing, filtering and sorting.
3. Identify and handle missing data using appropriate pandas methods.
4. Combine datasets using concatenation, joining and merging techniques.

## Notebook contents

| File | Topic | Lesson 6 slides | Suggested time |
|---|---|---|---|
| `pandas_walkthrough.ipynb` | Complete runnable demonstration | 9–109 | 30–40 min |
| `series_student_scores.ipynb` | Series, labels, `.loc` / `.iloc`, alignment | 20–21 | 15–20 min |
| `dataframe_ranking.ipynb` | DataFrame, rank, filter, sort, derived column | 40–41 | 20–25 min |
| `missing_data.ipynb` | `isna`, `fillna`, median, sentinel, interpolation | 61–63 | 20–25 min |
| `combine_tables.ipynb` | `concat`, `merge`, `join`, unmatched keys, validation | 89–91 | 25–30 min |
| `retail_analytics.ipynb` | Integrated, auditable retail revenue analysis | 96–102 | 25–35 min |

## Getting started

**Option A — JupyterLab locally:**

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Open a notebook under `notebooks/`, then run its cells from the top.

**Option B — Google Colab:** Open the `.ipynb` directly from the course GitHub repository in Colab. NumPy and pandas are normally available already.

## How to work with the activity notebooks

- Read each **Task**, complete the `# TODO` code and run the cell.
- Run the next **Self-check** cell. `PENDING` means you have not completed the task; `PASS` means your result meets that check.
- Explain your output in plain English. A passing checkpoint does not replace interpretation.
- All datasets are generated inside the notebooks. **No external files, credentials or network requests are required.**
- If you get unexpected results, restart the kernel and **Run All** to check for out-of-order execution.

## Instructor note

This folder does **not** contain the completed task-by-task instructor solution notebooks. The `00_` classroom walkthrough **does** contain fully worked examples using the lesson datasets, so upload it only if you want students to have that reference. Keep the instructor-solution package private.

## Course context

COM7024 Programming for Data Analytics · Week 6 · pandas Series, DataFrames, missing data, merging/joining/concatenation. Examples and success criteria follow the Week 6 teaching deck.
