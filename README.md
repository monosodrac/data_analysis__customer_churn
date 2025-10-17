[PYTHON_BADGE]:https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[PANDAS_BADGE]:https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white
[NUMPY_BADGE]:https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white
[PRS_BADGE]:https://img.shields.io/badge/PRs-welcome-green?style=for-the-badge

<h1 align="center" style="font-weight: bold;">Customer Churn Analysis with Python 🧠</h1>

![python][PYTHON_BADGE]
![pandas][PANDAS_BADGE]
![numpy][NUMPY_BADGE]
![prs][PRS_BADGE]

<details open="open">
<summary>Table of Contents</summary>
  
- [🚀 Getting started](#started)
  - [Prerequisites](#prerequisites)
  - [Cloning](#cloning)
  - [Environment Setup](#environment)
  - [Starting](#starting)
- [📍 How It Works](#how-it-works)
- [📊 Key Insights](#key-insights)
- [📁 Dataset Structure](#csv)
- [🧰 Files Overview](#files)
- [🤝 How to Reach Me](#reach)
- [📫 How to Contribute](#contribute)

</details>

<p align="center">
  <b>A Python data analysis project to understand and reduce customer churn.</b>
</p>

---

<h2 id="started">🚀 Getting started</h2>

<h3 id="prerequisites">Prerequisites</h3>

- [Python 3.10+](https://www.python.org/downloads/)
- [pip](https://pip.pypa.io/en/stable/installation/)
- [Jupyter Notebook](https://jupyter.org/install)

<h3 id="cloning">Cloning</h3>

```bash
git clone https://github.com/monosodrac/data_analysis__customer_churn.git
cd data_analysis__customer_churn
```

<h3 id="environment">Environment Setup</h3>

Install dependencies:
```
pip install pandas numpy plotly openpyxl nbformat ipykernel
```

<h3 id="starting">Starting</h3>

1. Place the CSV dataset (`cancelamentos_sample.csv`) in the project folder.
2. Open the Jupyter Notebook:
```bash
jupyter notebook
```
3. In the browser interface, open inicial.ipynb.
4. Run the notebook cells sequentially to execute the analysis.

<h2 id="how-it-works">📍 How It Works</h2>

The project performs the following steps:
1. Import the dataset using pandas.
2. Remove irrelevant columns and handle missing values.
3. Explore the dataset to identify patterns and potential errors.
4. Analyze the churn column:
    - Count of customers who canceled
    - Proportion of churned vs. active customers
5. Visualize customer data with plotly.express histograms by feature colored by churn.
6. Identify main churn drivers:
    - Monthly contracts have the highest churn → offer discounts on Annual/Quarterly plans
    - More than 4 call center calls → alert at 3 calls to prevent churn
    - Payment delays over 20 days → alert after 10 days
7. Simulate churn reduction by filtering:
    - Remove monthly contracts
    - Limit call-center calls ≤4
    - Limit payment delays ≤20 days
  
<h2 id="key-insights">📊 Key Insights</h2>

1. Initial churn rate: 56.7%
2. After filtering risky segments: churn drops to 18.4%
3. Major risk factors:
     - Monthly contracts
     - 4 call center interactions
     - Payment delays more than 20 days

<h2 id="csv">📁 Dataset Structure</h2>

| Column                   | Description                                    |
| ------------------------ | ---------------------------------------------- |
| `idade`                  | Customer age                                   |
| `sexo`                   | Gender                                         |
| `tempo_como_cliente`     | Time as a customer (months)                    |
| `frequencia_uso`         | Usage frequency                                |
| `ligacoes_callcenter`    | Number of call center calls                    |
| `dias_atraso`            | Payment delay in days                          |
| `assinatura`             | Subscription type (Basic, Standard, Premium)   |
| `duracao_contrato`       | Contract duration (Monthly, Quarterly, Annual) |
| `total_gasto`            | Total spent by the customer                    |
| `meses_ultima_interacao` | Months since last interaction                  |
| `cancelou`               | Churn indicator (1 = Yes / 0 = No)             |

<h2 id="files">🧰 Files Overview</h2>

| File                       | Description                                                         |
| -------------------------- | ------------------------------------------------------------------- |
| `inicial.ipynb`        | Main script: loads dataset, cleans, visualizes, and analyzes churn. |
| `cancelamentos_sample.csv` | Example dataset with customer information.                          |

<h2 id="reach">🤝 How to reach me</h2>

<table>
  <tr>
    <td align="center">
      <a href="https://linktr.ee/monosodrac">
        <img src="https://avatars.githubusercontent.com/u/141099551?v=4" width="100px;" alt="Mono Cardoso Profile Picture"/><br>
        <sub>
          <b>Mono</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

<h2 id="contribute">📫 Contribute</h2>

Contributions are welcome! 🧩  
If you’d like to help improve this automation or add new features, follow the steps below:

1. Clone the repository  
```bash
git clone https://github.com/monosodrac/data_analysis__customer_churn.git
```
2. Create a new branch for your feature or fix 
```bash
git checkout -b feature/your-feature-name
```
3. Follow good commit message practices
4. After implementing your change, open a Pull Request describing:
   - The problem solved or the feature added
   - Steps to test the modification
   - (If applicable) screenshots or short videos showing the automation working
Once your PR is submitted, wait for code review and feedback! 🚀

<h3>Documentations that might help</h3>

[📝 How to create a Pull Request](https://www.atlassian.com/br/git/tutorials/making-a-pull-request)

[💾 Commit pattern](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)
