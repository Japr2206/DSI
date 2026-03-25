# Dynamic Stability Index for Early Learning-Rate Selection

This repository contains the code, manuscript, and supporting materials for the study on the **Dynamic Stability Index (DSI)** as an interpretable early criterion for learning-rate selection in deep learning.

## Repository contents

The repository currently includes the following main files:

- **`DYNAMIC_STABILITY_INDEX_FOR_EARLY_LEARNING_RATE_SELECTION.ipynb`**  
  Main notebook containing the complete experimental workflow.

- **`requirements_v3.txt`**  
  Main dependency file for the project.

---

## Recommended reading order

For a first reading, the most useful order is:

1. **Read the manuscript PDF first.**  
   This provides the scientific context, the methodological motivation, and the interpretation of the results.

2. **Inspect the notebook in GitHub preview mode.**  
   GitHub renders the notebook with printed outputs, intermediate tables, and execution traces, which makes it possible to understand much of the workflow directly in the browser.

3. **Open the notebook in Google Colab if needed.**  
   The notebook can be opened from GitHub in Colab for interactive inspection or execution.

---

## What the notebook does

The notebook is designed as a **full experimental notebook**, not as a minimal illustrative example.

It implements the study end-to-end, including:

- project setup and configuration,
- dataset preparation,
- model definitions,
- training and evaluation functions,
- DSI computation,
- baseline learning-rate selection methods,
- robustness and sensitivity analyses,
- final model training,
- and export of tables, figures, and summary outputs.

Because of this structure, the notebook should be understood as a **computational laboratory notebook accompanying the manuscript**.

---

## General execution workflow

To run the project:

1. Open the notebook in **Google Colab**.
2. Install the dependencies from `requirements_v3.txt` if needed.
3. Mount Google Drive if persistent storage is required.
4. Verify the configured root paths for:
   - project directory,
   - output directory,
   - cached data directory.
5. Run the notebook sequentially from the first block to the last block.

### Important note

This is not a lightweight script. The notebook is organized so that:

- datasets are downloaded or prepared,
- exploratory sweeps are executed,
- DSI-based selection is computed,
- baselines are evaluated,
- final models are trained,
- tables and figures are generated,
- and outputs are saved to persistent folders.

For this reason:

- execution may take considerable time,
- some experiments benefit from GPU availability,
- and several later result blocks depend on earlier blocks having completed successfully.

If you do not want to rerun the full pipeline from scratch, the repository already includes the generated materials in **`Paper outputs_from_code.zip`**.

---

## How to interpret the repository

This repository is organized as a three-layer reproducibility structure:

- **Manuscript** = scientific narrative, methodology, and interpretation  
- **Notebook** = executable implementation of the pipeline  
- **Generated outputs** = preserved computational evidence arising from execution

In practical terms:

- the **manuscript** explains what is being measured and why it matters,
- the **notebook** shows how the results are produced,
- and **`Paper outputs_from_code.zip`** preserves the generated artifacts.

---


## Reproducibility notes

The experiments were implemented in Python with a Colab-oriented workflow and rely on common scientific and machine learning libraries, including **PyTorch** and **Scikit-learn**.

The notebook uses fixed seeds and organized output directories to improve reproducibility and output traceability.

Even so, as in most machine learning and deep learning experiments, minor run-to-run variations may still occur depending on:

- hardware,
- CUDA availability,
- package versions,
- and execution environment.

For that reason, the repository provides both:

- the code required to reproduce the pipeline,
- and the generated outputs corresponding to the reported version of the study.

---

## Availability

Is here :) - enjoy my humble contribution 
