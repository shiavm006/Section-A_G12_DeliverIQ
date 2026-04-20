# NST DVA Capstone 2 - Project Repository

> **Newton School of Technology | Data Visualization & Analytics**
> A 2-week industry simulation capstone using Python, GitHub, and Tableau to convert raw data into actionable business intelligence.

---

## Before You Start

1. Rename the repository using the format `SectionName_TeamID_ProjectName`.
2. Fill in the project details and team table below.
3. Add the raw dataset to `data/raw/`.
4. Complete the notebooks in order from `01` to `05`.
5. Publish the final dashboard and add the public link in `tableau/dashboard_links.md`.
6. Export the final report and presentation as PDFs into `reports/`.

### Quick Start

If you are working locally:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

If you are working in Google Colab:

- Upload or sync the notebooks from `notebooks/`
- Keep the final `.ipynb` files committed to GitHub
- Export any cleaned datasets into `data/processed/`

---

## Project Overview


| Field               | Details                                    |
| ------------------- | ------------------------------------------ |
| **Project Title**   | *To be filled by team*                     |
| **Sector**          | *e.g. Retail, Finance, Healthcare, EdTech* |
| **Team ID**         | *e.g. DVA-B1-T3*                           |
| **Section**         | *To be filled by team*                     |
| **Faculty Mentor**  | *To be filled by team*                     |
| **Institute**       | Newton School of Technology                |
| **Submission Date** | *To be filled by team*                     |


### Team Members


| Role                 | Name   | GitHub Username |
| -------------------- | ------ | --------------- |
| Project Lead         | *Name* | `github-handle` |
| Data Lead            | *Name* | `github-handle` |
| ETL Lead             | *Name* | `github-handle` |
| Analysis Lead        | *Name* | `github-handle` |
| Visualization Lead   | *Name* | `github-handle` |
| Strategy Lead        | *Name* | `github-handle` |
| PPT and Quality Lead | *Name* | `github-handle` |


---

## Business Problem

*Describe the sector context, the decision-maker this project serves, and the core business challenge being addressed. Keep this to 3-5 sentences written in plain language, as if addressing a senior stakeholder.*

**Core Business Question**

> *State the single main question your Tableau dashboard and Python analysis will answer.*

**Decision Supported**

> *What action or decision will this analysis enable the stakeholder to take?*

---

## Dataset


| Attribute               | Details                                           |
| ----------------------- | ------------------------------------------------- |
| **Source Name**         | *e.g. World Bank, data.gov.in, Kaggle (raw only)* |
| **Direct Access Link**  | *Paste the direct download or access URL*         |
| **Row Count**           | *Must be greater than 5,000*                      |
| **Column Count**        | *Must be greater than 8 meaningful columns*       |
| **Time Period Covered** | *e.g. Jan 2019 to Dec 2023*                       |
| **Format**              | *e.g. CSV, JSON, Excel*                           |


**Key Columns Used**


| Column Name | Description     | Role in Analysis                       |
| ----------- | --------------- | -------------------------------------- |
| *column_1*  | *What it means* | *Used for KPI / filter / segmentation* |
| *column_2*  | *What it means* | *Used for KPI / filter / segmentation* |
| *column_3*  | *What it means* | *Used for KPI / filter / segmentation* |
| *column_4*  | *What it means* | *Used for KPI / filter / segmentation* |


For full column definitions, see `[docs/data_dictionary.md](docs/data_dictionary.md)`.

---

## KPI Framework


| KPI                             | Definition                          | Formula / Computation                          |
| ------------------------------- | ----------------------------------- | ---------------------------------------------- |
| *e.g. Monthly Revenue Growth %* | *What business outcome this tracks* | *Show the exact formula or notebook reference* |
| *e.g. Customer Churn Rate*      | *What business outcome this tracks* | *Show the exact formula or notebook reference* |
| *e.g. Repeat Purchase Rate*     | *What business outcome this tracks* | *Show the exact formula or notebook reference* |


Document KPI logic clearly in `notebooks/04_statistical_analysis.ipynb` and `notebooks/05_final_load_prep.ipynb`.

---

## Tableau Dashboard


| Item                 | Details                                    |
| -------------------- | ------------------------------------------ |
| **Dashboard URL**    | *Paste Tableau Public link here*           |
| **Executive View**   | *Describe the high-level KPI summary view* |
| **Operational View** | *Describe the detailed drill-down view*    |
| **Main Filters**     | *List the interactive filters used*        |


Store dashboard screenshots in `[tableau/screenshots/](tableau/screenshots/)` and document the public links in `[tableau/dashboard_links.md](tableau/dashboard_links.md)`.

---

## Key Insights

*List 8-12 major findings from the analysis, written in decision language. Each insight should tell the reader what to think or act upon, not merely describe a chart.*

1. *Insight 1*
2. *Insight 2*
3. *Insight 3*
4. *Insight 4*
5. *Insight 5*
6. *Insight 6*
7. *Insight 7*
8. *Insight 8*

---

## Recommendations

*Provide 3-5 specific, actionable business recommendations, each linked directly to an insight above.*


| #   | Insight                            | Recommendation                    | Expected Impact                         |
| --- | ---------------------------------- | --------------------------------- | --------------------------------------- |
| 1   | *Which insight does this address?* | *What should the stakeholder do?* | *What measurable impact do you expect?* |
| 2   | *Which insight does this address?* | *What should the stakeholder do?* | *What measurable impact do you expect?* |
| 3   | *Which insight does this address?* | *What should the stakeholder do?* | *What measurable impact do you expect?* |


---

## Repository Structure

```text
SectionName_TeamID_ProjectName/
|
|-- README.md
|
|-- data/
|   |-- raw/                         # Original dataset (never edited)
|   `-- processed/                   # Cleaned output from ETL pipeline
|
|-- notebooks/
|   |-- 01_extraction.ipynb
|   |-- 02_cleaning.ipynb
|   |-- 03_eda.ipynb
|   |-- 04_statistical_analysis.ipynb
|   `-- 05_final_load_prep.ipynb
|
|-- scripts/
|   `-- etl_pipeline.py
|
|-- tableau/
|   |-- screenshots/
|   `-- dashboard_links.md
|
|-- reports/
|   |-- README.md
|   |-- project_report_template.md
|   `-- presentation_outline.md
|
|-- docs/
|   `-- data_dictionary.md
|
|-- DVA-oriented-Resume/
`-- DVA-focused-Portfolio/
```

---

## Analytical Pipeline

The project follows a structured 7-step workflow:

1. **Define** - Sector selected, problem statement scoped, mentor approval obtained.
2. **Extract** - Raw dataset sourced and committed to `data/raw/`; data dictionary drafted.
3. **Clean and Transform** - Cleaning pipeline built in `notebooks/02_cleaning.ipynb` and optionally `scripts/etl_pipeline.py`.
4. **Analyze** - EDA and statistical analysis performed in notebooks `03` and `04`.
5. **Visualize** - Interactive Tableau dashboard built and published on Tableau Public.
6. **Recommend** - 3-5 data-backed business recommendations delivered.
7. **Report** - Final project report and presentation deck completed and exported to PDF in `reports/`.

---

## Tech Stack


| Tool                       | Status    | Purpose                                            |
| -------------------------- | --------- | -------------------------------------------------- |
| Python + Jupyter Notebooks | Mandatory | ETL, cleaning, analysis, and KPI computation       |
| Google Colab               | Supported | Cloud notebook execution environment               |
| Tableau Public             | Mandatory | Dashboard design, publishing, and sharing          |
| GitHub                     | Mandatory | Version control, collaboration, contribution audit |
| SQL                        | Optional  | Initial data extraction only, if documented        |


**Recommended Python libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`

---

## Evaluation Rubric


| Area                        | Marks   | Focus                                                       |
| --------------------------- | ------- | ----------------------------------------------------------- |
| Problem Framing             | 10      | Is the business question clear and well-scoped?             |
| Data Quality and ETL        | 15      | Is the cleaning pipeline thorough and documented?           |
| Analysis Depth              | 25      | Are statistical methods applied correctly with insight?     |
| Dashboard and Visualization | 20      | Is the Tableau dashboard interactive and decision-relevant? |
| Business Recommendations    | 20      | Are insights actionable and well-reasoned?                  |
| Storytelling and Clarity    | 10      | Is the presentation professional and coherent?              |
| **Total**                   | **100** |                                                             |


> Marks are awarded for analytical thinking and decision relevance, not chart quantity, visual decoration, or code length.

---

## Submission Checklist

**GitHub Repository**

- Public repository created with the correct naming convention (`SectionName_TeamID_ProjectName`)
- All notebooks committed in `.ipynb` format
- `data/raw/` contains the original, unedited dataset
- `data/processed/` contains the cleaned pipeline output
- `tableau/screenshots/` contains dashboard screenshots
- `tableau/dashboard_links.md` contains the Tableau Public URL
- `docs/data_dictionary.md` is complete
- `README.md` explains the project, dataset, and team
- All members have visible commits and pull requests

**Tableau Dashboard**

- Published on Tableau Public and accessible via public URL
- At least one interactive filter included
- Dashboard directly addresses the business problem

**Project Report**

- Final report exported as PDF into `reports/`
- Cover page, executive summary, sector context, problem statement
- Data description, cleaning methodology, KPI framework
- EDA with written insights, statistical analysis results
- Dashboard screenshots and explanation
- 8-12 key insights in decision language
- 3-5 actionable recommendations with impact estimates
- Contribution matrix matches GitHub history

**Presentation Deck**

- Final presentation exported as PDF into `reports/`
- Title slide through recommendations, impact, limitations, and next steps

**Individual Assets**

- DVA-oriented resume updated to include this capstone
- Portfolio link or project case study added

---

## Contribution Matrix

This table must match evidence in GitHub Insights, PR history, and committed files.


| Team Member | Dataset and Sourcing | ETL and Cleaning  | EDA and Analysis  | Statistical Analysis | Tableau Dashboard | Report Writing    | PPT and Viva      |
| ----------- | -------------------- | ----------------- | ----------------- | -------------------- | ----------------- | ----------------- | ----------------- |
| *Member 1*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |
| *Member 2*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |
| *Member 3*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |
| *Member 4*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |
| *Member 5*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |
| *Member 6*  | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support*    | *Owner / support* | *Owner / support* | *Owner / support* |


*Declaration: We confirm that the above contribution details are accurate and verifiable through GitHub Insights, PR history, and submitted artifacts.*

**Team Lead Name:** _____________________________

**Date:** _______________

---

## Academic Integrity

All analysis, code, and recommendations in this repository must be the original work of the team listed above. Free-riding is tracked via GitHub Insights and pull request history. Any mismatch between the contribution matrix and actual commit history may result in individual grade adjustments.

---

*Newton School of Technology - Data Visualization & Analytics | Capstone 2*