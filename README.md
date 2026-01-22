# Global AI Job Market Analysis

> **An interactive visualization dashboard analyzing salary trends, skill demands, and the global adoption of Artificial Intelligence in the labor market.**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://data-visualization---projectapp-xdv3vriyf7wojgvtaqlwva.streamlit.app)

![Dashboard Preview](image_6684d2.png)

## About
The rise of Artificial Intelligence has fundamentally transformed the global workforce. This project explores the "AI revolution" through data, providing a comprehensive dashboard built with **Streamlit** and **Plotly**.

It allows users to analyze real-time data, compare different countries, understand salary distributions across experience levels, and identify which technical skills yield the highest return on investment.

---

## Key Features & Pages

The application is divided into four distinct analysis modules:

### 1. Global AI Adoption Landscape (`Home.py`)
**The Main Hub & Geographic Analysis.**
* **Interactive World Map:** Visualizes job distribution by **Company Location** or **Employee Residence**.
* **Country Comparison Tool:** Allows side-by-side comparison of two countries (Primary vs. Secondary) based on average salary, remote work ratios, and market dominance.
* **Top 10 Rankings:** Breakdowns of the leading countries and most popular job titles.

### 2. Salary Distribution by Job Title
**Deep Dive into Compensation.**
* **Scatter Plot Analysis:** Visualizes salaries (USD) across different job titles and countries.
* **Experience Filtering:** Color-coded data points distinguishing between Entry-level, Mid-level, Senior, and Executive roles.
* **Gap Analysis:** Highlights significant salary disparities for similar roles in different geographic regions.

### 3. The AI Skill Wars
**Demand vs. Value Analysis.**
* **Quadrant Chart:** Maps technical skills on two axes: **Popularity (Frequency)** vs. **Average Salary**.
* **Strategic Insights:** Categorizes skills into four segments:
    * **Hidden Gems:** High salary, lower competition.
    * **Core Skills:** High salary, high demand.
    * **Niche:** Lower demand, lower salary.
    * **Commoditized:** High demand, lower salary.

### 4. Multidimensional Comparative Analysis
**Smart Job Ranking System.**
* **Min-Max Normalization:** A custom algorithm that scores job roles based on three weighted metrics:
    1.  **Salary Potential**
    2.  **Job Frequency (Demand)**
    3.  **Remote Work Availability**
* **Unified Score:** Generates a single metric (0 to 1) to objectively rank the "best" AI jobs in the current market.

---

## Tech Stack
* **Language:** Python 3.x
* **Framework:** [Streamlit](https://streamlit.io/)
* **Visualization:** Plotly Express & Graph Objects
* **Data Manipulation:** Pandas

---

## Installation & Local Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/YourRepoName.git](https://github.com/YourUsername/YourRepoName.git)
    cd YourRepoName
    ```

2.  **Install dependencies:**
    ```bash
    pip install streamlit pandas plotly
    ```

3.  **Run the application:**
    ```bash
    streamlit run Home.py
    ```

---

## Project Structure

```text
├── Home.py                                            # Main application entry point
├── ai_job_dataset - all.csv                           # Raw dataset
├── pages/
│   ├── Salary Distribution by Job Title (USD).py      # Salary analysis page
│   ├── AI Skills Landscape in the Job Market...py     # Skills analysis page
│   └── A multidimensional comparative analysis...py   # Job ranking/scoring page
├── image_6684d2.png                                   # Project image/logo
└── README.md                                          # Documentation
