# 📌 Circular Task Analysis – MouseReMoCo

## ✅ Project Overview

This project focuses on the analysis of **circular target tasks** recorded using the **MouseReMoCo** system. The primary goals are to understand the experimental data structure, reproduce key visualizations, compute standard performance metrics, and validate the analysis against provided and self-generated data.

### Goals:

* Understand how the **MouseReMoCo** data is structured and recorded.
* Reproduce **trajectory and time-series plots** for the task. 
* Compute and analyze performance metrics, including:
    * **$nLaps$**: Number of completed laps.
    * **$Re$**: Effective radius.
    * **$Te$**: Effective time.
    * **$error\%$**: Percentage of time/distance outside the target area.
    * **$MT/lap$**: Movement time per lap.
    * **$IDe/lap$**: Effective Index of Difficulty per lap.
    * **$Be$**: Effective bandwidth.
    * **$IPe$**: Effective index of performance.
* Validate results against provided reference data and apply the analysis to self-generated data.

---

## ✅ Repository Structure

The repository is structured as follows:

├── data/ # Contains provided and self-generated CSV files 
├── circular_task_analysis/circular_task_analysis.ipynb # Jupyter notebook containing all   analysis code 
├── README.md # This project documentation file 
└── report.pdf # Final report summarizing findings (1–2 pages)

---

## ✅ Getting Started

### How to Run

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/](https://github.com/)<your-username>/<repo-name>.git
    cd <repo-name>
    ```

2.  **Install dependencies:**

    This project requires **NumPy** for numerical operations and **Matplotlib** for visualization.

    ```bash
    pip install numpy matplotlib
    ```

3.  **Run the analysis:**

    The full analysis is contained within a Jupyter Notebook.

    ```bash
    jupyter notebook circular_task_analysis/circular_task_analysis.ipynb
    ```

    Open the notebook `circular_task_analysis.ipynb` and execute the cells in sequential order.

---

## ✅ Key Features

The analysis pipeline in the notebook includes:

* **Data Loading & Parsing:** Functions to read kinematic data and marker files, extract record ranges, and compute relative coordinates.
* **Visualization:**
    * **Trajectory plots** showing inside/outside target points.
    * **Time-series plots** for X, Y, and the inside-target flag.
* **Metrics Computation:** Automated calculation of the following key metrics:
    * $nLaps$
    * $Re$
    * $Te$
    * $error\%$
    * $MT/lap$
    * $IDe/lap$
    * $Be$
    * $IPe$
* **Own Data Analysis:** Applying the established processing and analysis pipeline to self-generated data collected with **MouseReMoCo**.

---

## ✅ Expected Outputs

Executing the notebook will generate the following outputs:

* **Trajectory and time-series plots** for each analyzed record.
* A **metrics table** summarizing performance for both professor-provided data and own generated data.
* A **brief report** (`report.pdf`) summarizing the methodology, challenges encountered, and solutions implemented.

---

## ✅ Team Contributions

The project was developed collaboratively with the following roles and contributions:

* **Manager:**
    * Created the GitHub repository, managed branches, and handled merges.
    * Implemented the metrics computation and the analysis pipeline for own data (Notebook Cells \[8]–\[9]).
* **Teammate A:**
    * Implemented data loading and preprocessing functions (Notebook Cells \[1]–\[4]).
* **Teammate B:**
    * Implemented visualization and plotting functions (Notebook Cells \[5]–\[7]).