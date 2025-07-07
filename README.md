# Post-Pandemic-Remote-Work-Health-Impact-2025
A Python Data Analytics project that investigates how the shift to remote and hybrid work models following the COVID-19 pandemic has influenced employees' mental and physical health, burnout levels, work-life balance, and overall well-being. 

## Introduction

In the aftermath of COVID-19, organizations worldwide adopted remote and hybrid work models at an unprecedented scale. While these changes brought flexibility and safety, they also introduced new challenges—social isolation, blurred work-life boundaries, and rising mental health concerns.

This project was initiated to explore one critical question: **How has the post-pandemic work environment impacted employee well-being and burnout?**

## Project Overview

This project investigates the impact of remote, hybrid, and onsite work arrangements on employee well-being in the post-pandemic era. Using Python and advanced data analysis techniques, it explores how different workplace structures relate to burnout, mental health conditions, physical health issues, work-life balance, and social isolation.

The analysis is based on a **synthetic yet realistic dataset** representing survey responses from over 2,000 employees across various regions, industries, and job roles. The dataset includes both numerical and categorical variables capturing work patterns, demographics, health indicators, and perceived satisfaction metrics.

Through rigorous data cleaning, transformation, and multi-dimensional visual exploration using **Pandas**, **Seaborn**, and **Matplotlib**, this project answers strategic questions relevant to HR leaders, organizational psychologists, and future-of-work researchers.

**Key areas of analysis include:**
- The relationship between **work arrangements** and mental health conditions
- Factors contributing to **burnout severity** (e.g., gender, hours, age, salary)
- Prevalence of **physical health issues** by industry and role
- The influence of **social isolation** and **work-life balance** on well-being
- How **salary and geographic region** shape mental health and burnout trends

The insights uncovered are presented through clean, publication-ready visualizations and interpreted with business relevance in mind, making this project not only analytically rigorous but also practically useful.

## Project Scope

This project is focused on **exploratory data analysis (EDA)** of a simulated post-pandemic employee well-being dataset. It aims to uncover how workplace factors influence mental and physical health, burnout, and work-life balance in 2025.

**In Scope**
- Analysis of the relationship between:
  - **Work arrangements** (remote, hybrid, onsite) and **mental health conditions**
  - **Burnout levels** by gender, age group, working hours, and salary
  - **Physical health issues** across industries and job types
  - **Social isolation and work-life balance** as predictors of employee stress
  - **Salary and geographic region** as influences on burnout and emotional well-being
- Cleaning and preprocessing of multi-response survey fields (e.g. health issues)
- Data transformation using `explode()`, `groupby()`, and binning for better insights
- Visualizations using **Seaborn** and **Matplotlib**:
  - Grouped bar charts
  - Heatmaps
  - Box plots
- Human-centered interpretation of findings with relevance to **HR strategy** and **wellness design**

**Out of Scope**

- No machine learning or predictive modeling
- No real-time dashboards (e.g. Streamlit, Tableau)
- No time-series forecasting (dataset does not contain temporal features)
- No NLP or sentiment analysis (dataset is structured/tabular)

**Time Frame & Dataset Size**

- **Dataset:** Synthetic CSV file with ~2,000 employee records  
- **Scope of Analysis:** One-time snapshot for the simulated year **2025**

**Intended Audience**

- HR professionals & people analytics teams
- Organizational psychologists
- Data science learners focusing on applied EDA
- Employers designing remote/hybrid workplace policies

## Business Objectives

- Understand how work arrangements (remote, hybrid, in-office) impact mental health.
- Identify factors most associated with burnout (e.g., gender, working hours, age, isolation).
- Determine which physical health issues are prevalent and how they vary across industries.
- Analyze the relationship between salary, region, and employee well-being.
- Investigate the role of work-life balance and social isolation in shaping burnout and mental health.
- Generate insights that can support HR and organizational wellness strategy.

## Use Case

- **HR Teams**: Identify high-risk groups for burnout and mental health issues to target wellness programs.
- **Organizational Leaders**: Understand the effects of remote/hybrid policies on employee satisfaction and isolation.
- **Data Analysts**: Use the code structure as a reference for EDA best practices on survey-style data.
- **Students & Researchers**: Explore real-world survey design themes, multi-label processing, and workplace analytics use cases.

## Data Source

This dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/pratyushpuri/remote-work-health-impact-survey-2025), where it was published as a synthetic survey representing employee experiences with remote work in 2025. It was created to reflect real-world trends in burnout, mental health, work-life balance, and physical well-being — and serves as a strong foundation for exploratory analysis in organizational health and remote work research.

## Dataset Overview
**Tools, Technologies & Dataset**

This project integrates Python-based data science tools to explore the relationship between work arrangements and employee well-being in the post-pandemic era. The following tools and technologies were used:

| Tool / Library              | Purpose                                                                 |
|----------------------------|-------------------------------------------------------------------------|
| **Python (Pandas, NumPy)** | Data loading, cleaning, manipulation, and aggregation                  |
| **Matplotlib & Seaborn**   | Data visualization through bar charts, heatmaps, and distribution plots |
| **Google Colab / Jupyter** | Interactive coding environment for exploratory analysis and visualization |
| **Markdown / GitHub**      | Project documentation and version control                              |

---

**Dataset Overview**

| Feature                     | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **File name**               | `post_pandemic_remote_work_health_impact_2025.csv`                          |
| **Data type**               | Synthetic dataset (based on realistic post-pandemic employee surveys)       |
| **Records**                 | ~2,000 rows of anonymized employee responses                               |
| **Dimensions**              | 16 columns including categorical, numerical, and multi-response fields      |
| **Collection year**         | Simulated for the year 2025                                                |

---

**Key Variables in the Dataset**

| Column Name                  | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| `Work_Arrangement`           | Work mode: Remote, Hybrid, or Onsite                                        |
| `Mental_Health_Status`       | Multi-label mental health conditions (e.g. Anxiety, Depression, Burnout)    |
| `Burnout_Level`              | Severity level of burnout: Low, Medium, High                                |
| `Physical_Health_Issues`     | Multi-label issues like Back Pain, Eye Strain, Neck Pain                    |
| `Work_Life_Balance_Score`    | Self-rated score (1–10) indicating satisfaction with work-life balance       |
| `Social_Isolation_Score`     | Self-reported isolation (1–10), higher = more isolated                      |
| `Salary_Range`               | Employee’s annual salary category (e.g. <$60K, $100K–$120K, etc.)           |
| `Industry`                   | Employee’s industry of work                                                 |
| `Region`                     | Geographic region of respondent (e.g. Asia, Europe, Africa)                 |
| `Age`, `Gender`, `Hours_Per_Week` | Demographics and work characteristics                              |

---

**Why a Synthetic Dataset?**

To simulate realistic trends while preserving privacy, the dataset was **synthetically generated based on common global patterns** in remote work and health studies post-COVID-19. It mirrors the kind of data HR teams, researchers, or policy analysts might use to guide decision-making in 2025.

## Data Cleaning and Processing 

Before analysis, the dataset was cleaned and prepared to ensure consistency, accuracy, and analysis-readiness. Key data preparation steps included:

**Handling Missing and Placeholder Values**
- Removed records with `"None"` values in critical fields such as `Mental_Health_Status` and `Physical_Health_Issues`.
- Ensured no empty strings or nulls interfered with grouping and aggregation.

**Exploding Multi-Label Fields**
- Fields like `Mental_Health_Status` and `Physical_Health_Issues` contained multiple responses separated by semicolons (`;`).
- These were split and **exploded into individual rows** using `str.split('; ')` and `explode()`, allowing for accurate frequency analysis by condition or symptom.

**Binning & Categorization**
- **Age** was grouped into defined ranges (e.g. 18–25, 26–35, 36–45, etc.) to explore trends across life stages.
- **Working hours** (`Hours_Per_Week`) were categorized into 5 custom bins to detect burnout thresholds:
  - `<20`, `21–35`, `36–45`, `46–60`, `60+`
- This allowed for clearer interpretation in bar charts and grouped comparisons.

**Standardizing Categorical Data**
- Uniformed values in columns like `Work_Arrangement`, `Burnout_Level`, and `Gender` to prevent duplicates due to typos or inconsistent casing.
- Checked for and removed any duplicate rows.

**Creating Derived Fields**
- Added new columns such as:
  - `Age_Group` (from `Age`)
  - `Hours_Group` (from `Hours_Per_Week`)
- These helped simplify visualizations and interpret group-based trends more easily.

---

The result was a **clean, structured DataFrame** ready for targeted analysis by demographic, regional, and health-related dimensions.

## Key Analysis and Insights
**Q1. What types of mental health issues are more common for each work arrangement?**

**Objective**
To identify how different work environments — **Remote**, **Hybrid**, and **Onsite** — influence the type and frequency of mental health issues reported by employees.

This analysis helps organizations tailor **mental wellness support** to specific working conditions.

---

**Key Findings**

After cleaning and exploding multi-response entries from the `Mental_Health_Status` column, we found the following:

| Work Arrangement | Top Mental Health Issues                 | Notable Counts                       |
|------------------|-------------------------------------------|--------------------------------------|
| **Onsite**       | Burnout, Depression, PTSD                 | Burnout (80), Depression (78), PTSD (65) |
| **Hybrid**       | Anxiety, Burnout, Depression              | Anxiety (72), Burnout (70), Depression (65) |
| **Remote**       | Anxiety, Burnout, Isolation               | Anxiety (60), Burnout (55), Isolation (48) |

- **Onsite workers** reported the **highest number of severe psychological conditions** (e.g. PTSD, Depression).
- **Remote workers** showed higher incidence of **anxiety** and **isolation-related conditions**.
- **Hybrid workers** had a more balanced distribution, with moderately high levels across several conditions.

---

**Interpretation**

- **Onsite employees are most at risk** for intense, chronic stress and emotional strain — likely due to environmental factors, rigid schedules, and commuting.  
- **Remote workers**, while shielded from some stressors, are more vulnerable to **isolation** and **anxiety**, potentially due to lack of daily in-person connection.  
- **Hybrid work** appears to strike a balance, showing a **diversified but moderate risk profile**, supporting its reputation as a more sustainable long-term model.

---
```python
# Filter out 'None' values from mental health
mh_df = df[df["Mental_Health_Status"] != "None"].copy()

# Split multi-label responses
mh_df["Mental_Health_Status"] = mh_df["Mental_Health_Status"].str.split("; ")
mh_df = mh_df.explode("Mental_Health_Status")

# Group by Work Arrangement and Mental Health Status
mh_summary = mh_df.groupby(["Work_Arrangement", "Mental_Health_Status"]).size().reset_index(name="Count")

# Visualization
plt.figure(figsize=(12, 6))
sns.barplot(data=mh_summary, x="Work_Arrangement", y="Count", hue="Mental_Health_Status", palette="Set2")
plt.title("Mental Health Issues by Work Arrangement")
plt.xlabel("Work Arrangement")
plt.ylabel("Number of Cases")
plt.legend(title="Mental Health Condition", bbox_to_anchor=(1.05, 1), loc="upper left")
plt.tight_layout()
plt.show()
```

**Q2. What factors are most associated with high burnout levels?**

**Objective**

To identify which **demographic** and **workplace factors** are most strongly linked to high burnout. This helps employers understand where burnout risk is concentrated and develop targeted interventions.

---

**Analytical Steps & Insights**

**Step A: Burnout Level by Gender**

```python
burnout_by_gender = df[df["Mental_Health_Status"] == "Burnout"].groupby(["Gender", "Burnout_Level"]).size().reset_index(name="Count")

# Plot Burnout by Gender
plt.figure(figsize=(8, 5))
sns.barplot(data=gender_burnout, x="Gender", y="Count", hue="Burnout_Level", palette="flare")
plt.title("Burnout Levels by Gender")
plt.xlabel("Gender")
plt.ylabel("Number of Burnout Cases")
plt.legend(title="Burnout Level")
plt.tight_layout()
plt.show()
```

| Gender | High Burnout | Medium Burnout | Low Burnout | Total |
|--------|--------------|----------------|-------------|-------|
| Male   | 56           | 80             | 44          | 180   |
| Female | 53           | 83             | 48          | 184   |





