# Post-Pandemic-Remote-Work-Health-Impact-2025
A Python Data Analytics project that investigates how the shift to remote and hybrid work models following the COVID-19 pandemic has influenced employees' mental and physical health, burnout levels, work-life balance, and overall well-being. 

## Table of Contents
- [Introduction](#-introduction)
- [Project Overview](#-project-overview)
- [Project Scope](#-project-scope)
- [Business Objectives](#-business-objectives)
- [Use Case](#-use-case)
- [Data Source](#-data-source)
- [Dataset Overview](#-dataset-overview)
- [Data Cleaning & Processing](#-data-cleaning--processing)
- [Key Analysis and Insights](#-key-analysis-and-insights)
  - [Q1. What types of mental health issues are more common for each work arrangement?](#q1-what-types-of-mental-health-issues-are-more-common-for-each-work-arrangement)
  - [Q2. What factors are most associated with high burnout levels?](#q2-what-factors-are-most-associated-with-high-burnout-levels)
  - [Q3. Are there any notable physical health issues reported, and do they vary by industry or work arrangement?](#q3-are-there-any-notable-physical-health-issues-reported-and-do-they-vary-by-industry-or-work-arrangement)
  - [Q4. What role does social isolation play in burnout and mental health?](#q4-what-role-does-social-isolation-play-in-burnout-and-mental-health)
  - [Q5. Do salary and region influence employee well-being and burnout levels?](#q5-do-salary-and-region-influence-employee-well-being-and-burnout-levels)
  - [Q6. How does work-life balance correlate with burnout and mental health?](#q6-how-does-work-life-balance-correlate-with-burnout-and-mental-health)
- [Recommendations](#-recommendations)
- [Conclusion](#-conclusion)
- [Contact](#-contact)


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
### Q1. What types of mental health issues are more common for each work arrangement?

**Objective**
To identify how different work environments — **Remote**, **Hybrid**, and **Onsite** — influence the type and frequency of mental health issues reported by employees.

This analysis helps organizations tailor **mental wellness support** to specific working conditions.

---

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Mental%20Health%20Issues%20by%20Work%20Arrangement%20.png)


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

---

**Key Findings**

After cleaning and exploding multi-response entries from the `Mental_Health_Status` column, we found the following:

| Work Arrangement | Top Mental Health Issues                  | Notable Counts                         |
|------------------|-------------------------------------------|---------------------------------------|
| **Onsite**       | Burnout, Depression, PTSD                 | Burnout (80), Depression (78), PTSD (65)   |
| **Hybrid**       | Anxiety, Burnout, Depression              | Anxiety (72), Burnout (70), Depression (65) |
| **Remote**       | Anxiety, Burnout, Isolation               | Anxiety (60), Burnout (55), Isolation (48)  |

- **Onsite workers** reported the **highest number of severe psychological conditions** (e.g. PTSD, Depression).
- **Remote workers** showed higher incidence of **anxiety** and **isolation-related conditions**.
- **Hybrid workers** had a more balanced distribution, with moderately high levels across several conditions.

---

**Interpretation**

- **Onsite employees are most at risk** for intense, chronic stress and emotional strain — likely due to environmental factors, rigid schedules, and commuting.  
- **Remote workers**, while shielded from some stressors, are more vulnerable to **isolation** and **anxiety**, potentially due to lack of daily in-person connection.  
- **Hybrid work** appears to strike a balance, showing a **diversified but moderate risk profile**, supporting its reputation as a more sustainable long-term model.

---


### Q2. What factors are most associated with high burnout levels?

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

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20by%20Gender.png)

| Gender | High Burnout | Medium Burnout | Low Burnout | Total |
|--------|--------------|----------------|-------------|-------|
| Male   | 56           | 80             | 44          | 180   |
| Female | 53           | 83             | 48          | 184   |

**Interpretation:** Burnout is almost equally reported between genders, with slightly higher medium burnout among females.

---

**Step B: Burnout Level by Work Arrangement**

```python
burnout_by_arrangement = df[df["Mental_Health_Status"] == "Burnout"].groupby(["Work_Arrangement", "Burnout_Level"]).size().reset_index(name="Count")

# Plot Burnout by Work Arrangement
sns.barplot(data=burnout_by_arrangement, x="Work_Arrangement", y="Count", hue="Burnout_Level", palette="flare")
plt.title("Burnout Level by Work Arrangement")
plt.show()
```

https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20by%20work%20arrangement.png)

| Work Arrangement | High Burnout | Medium Burnout | Low Burnout | Total |
|------------------|--------------|----------------|-------------|--------|
| Remote           | 21           | 35             | 28          | 84     |
| Hybrid           | 42           | 53             | 27          | 122    |
| Onsite           | 46           | 55             | 63          | 164    |

**Interpretation:** Onsite employees had the highest total burnout, including high burnout cases. Hybrid workers showed a more moderate distribution.

---

**Step C: Burnout Level by Working Hours**

```python
df_burnout_hours = df[df["Mental_Health_Status"] == "Burnout"].copy()
df_burnout_hours["Hours_Group"] = pd.cut(df_burnout_hours["Hours_Per_Week"], bins=[0, 20, 35, 45, 60, 100], labels=["<20", "21–35", "36–45", "46–60", "60+"])
burnout_by_hours = df_burnout_hours.groupby(["Hours_Group", "Burnout_Level"]).size().reset_index(name="Count")

# Plot Burnout by Working Hours
plt.figure(figsize=(8, 5))
sns.barplot(data=hours_summary, x="Hours_Category", y="Count", hue="Burnout_Level", palette="mako")
plt.title("Burnout Levels by Working Hours")
plt.xlabel("Working Hours Per Week")
plt.ylabel("Number of Burnout Cases")
plt.legend(title="Burnout Level")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20by%20working%20hours.png)

| Hours Group | High Burnout | Medium Burnout | Low Burnout | Total |
|-------------|--------------|----------------|-------------|--------|
| <20         | 0            | 0              | 0           | 0      |
| 21–35       | 4            | 5              | 3           | 12     |
| 36–45       | 41           | 53             | 35          | 129    |
| 46–60       | 55           | 90             | 41          | 186    |
| 60+         | 19           | 30             | 16          | 65     |


**Interpretation:** Burnout peaks in the 46–60 hour/week range. It drops again at 60+, possibly due to autonomy, executive roles, or underreporting.

---

**Step D: Burnout Level by Age Group**

```python
df_burnout_age = df[df["Mental_Health_Status"] == "Burnout"].copy()
df_burnout_age["Age_Group"] = pd.cut(df_burnout_age["Age"], bins=[17, 25, 35, 45, 60, 100], labels=["18–25", "26–35", "36–45", "46–60", "60+"])
burnout_by_age = df_burnout_age.groupby(["Age_Group", "Burnout_Level"]).size().reset_index(name="Count")

# Plot Burnout by Age group
plt.figure(figsize=(8, 5))
sns.barplot(data=age_summary, x="Age_Group", y="Count", hue="Burnout_Level", palette="rocket")
plt.title("Burnout Levels by Age Group")
plt.xlabel("Age Group")
plt.ylabel("Number of Burnout Cases")
plt.legend(title="Burnout Level")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20by%20Age%20group.png)

| Age Group | High Burnout | Medium Burnout | Low Burnout | Total |
|-----------|--------------|----------------|-------------|--------|
| 18–25     | 12           | 14             | 7           | 33     |
| 26–35     | 29           | 37             | 20          | 86     |
| 36–45     | 27           | 55             | 25          | 107    |
| 46–60     | 36           | 58             | 32          | 126    |
| 60+       | 15           | 14             | 11          | 40     |


**Interpretation:** The 26–35 age group had the highest number of high burnout cases, supporting the idea that early-career professionals face intense pressure.

---

**Insights**

Burnout is not driven by a single factor — rather, it emerges from the intersection of personal demographics and workplace conditions. The analysis reveals some clear patterns:

Working hours are a major contributor: employees working 46–60 hours per week reported the highest number of high burnout cases (55). This suggests that sustained extended hours significantly increase emotional and physical strain, especially without adequate support.

Age plays a crucial role: the 26–35 age group reported the highest high burnout count (29). This demographic likely includes early- to mid-career professionals navigating career development, increased responsibilities, and life transitions — all of which contribute to pressure and fatigue.

Work arrangement matters: Onsite workers had the highest total burnout levels, including 46 high burnout cases. Unlike remote or hybrid settings, onsite roles may offer less flexibility, more commuting stress, and fewer opportunities for autonomy or personalized routines.

Gender, on the other hand, did not show a significant difference in burnout levels. Both males and females reported similar counts, indicating that burnout is more likely influenced by structural and role-related factors than by gender alone.

**Key takeaway:** The most vulnerable employees are those in high-demand roles, working long hours, often onsite, and in early or mid-career stages. Recognizing these burnout hotspots can help organizations deploy targeted wellness initiatives, reduce attrition, and foster healthier work environments.

### Q3. Are there any notable physical health issues reported, and do they vary by industry or work arrangement?

**Objective**

To explore whether certain physical health complaints (e.g. back pain, eye strain) are more common in specific **industries** or **work arrangements**. This analysis helps identify where **ergonomic risks** or **job-specific physical demands** are concentrated.

---

**Data Processing**

The `Physical_Health_Issues` column contains **multiple symptoms per employee**, separated by `; `. We used the `explode()` function to split and analyze them individually.

```python
# Filter out 'None' values
health_df = df[df["Physical_Health_Issues"] != "None"].copy()

# Explode multi-value column
health_df["Physical_Health_Issues"] = health_df["Physical_Health_Issues"].str.split("; ")
health_df = health_df.explode("Physical_Health_Issues")
```

---

**Step A: Top Reported Physical Health Issues**

```python
issue_counts = health_df["Physical_Health_Issues"].value_counts().reset_index()
issue_counts.columns = ["Physical_Health_Issue", "Count"]

plt.figure(figsize=(10, 5))
sns.barplot(data=issue_counts, x="Count", y="Physical_Health_Issue", palette="crest")
plt.title("Common Physical Health Issues (Exploded)")
plt.xlabel("Number of People")
plt.ylabel("Health Issue")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Common%20Physical%20Health%20Issues.png)


| Physical Health Issue | Count |
|------------------------|-------|
| Back Pain              | 287   |
| Eye Strain             | 263   |
| Neck Pain              | 217   |
| Wrist Pain             | 196   |
| Fatigue                | 188   |

**Interpretation:** The most frequently reported complaints are back pain and eye strain, both common in desk-bound, screen-heavy roles.

---

**Step B: Top Physical Health Issues by Industry**

```python
industry_issues = health_df.groupby(["Industry", "Physical_Health_Issues"]).size().reset_index(name="Count")

plt.figure(figsize=(12, 6))
sns.barplot(data=industry_issues, y="Industry", x="Count", hue="Physical_Health_Issues", palette="viridis")
plt.title("Physical Health Issues by Industry")
plt.xlabel("Number of People")
plt.ylabel("Industry")
plt.legend(title="Health Issue", bbox_to_anchor=(1.05, 1), loc="upper left")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Physical%20Health%20Issues%20by%20Industry.png)

| Industry              | Most Reported Issue | Count |
|-----------------------|----------------------|-------|
| Professional Services | Eye Strain           | 372   |
| Technology            | Back Pain            | 314   |
| Finance               | Eye Strain           | 192   |
| Manufacturing         | Back Pain            | 176   |
| Education             | Shoulder Pain        | 163   |
| Healthcare            | Eye Strain           | 130   |
| Marketing             | Back Pain            | 102   |
| Retail                | Eye Strain           | 97    |
| Customer Service      | Eye Strain           | 92    |

**Interpretation:** Eye strain is the most common issue across service and desk-based industries, while back pain dominates in more operational or sedentary roles like Technology and Manufacturing.
Education stands out with a higher rate of shoulder pain, possibly from posture, lifting, or multitasking duties.

---

**Step C: Top Physical Health Issues by Work Arrangement**

```python
arrangement_issues = health_df.groupby(["Work_Arrangement", "Physical_Health_Issues"]).size().reset_index(name="Count")

plt.figure(figsize=(10, 6))
sns.barplot(data=arrangement_issues, x="Work_Arrangement", y="Count", hue="Physical_Health_Issues", palette="coolwarm")
plt.title("Physical Health Issues by Work Arrangement")
plt.xlabel("Work Arrangement")
plt.ylabel("Number of People")
plt.legend(title="Health Issue", bbox_to_anchor=(1.05, 1), loc="upper left")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Physical%20Health%20Issues%20by%20work%20arrangement%20.png)

| Work Arrangement | Most Reported Issue | Count |
|------------------|----------------------|-------|
| Remote           | Eye Strain           | 96    |
| Hybrid           | Back Pain            | 102   |
| Onsite           | Back Pain            | 89    |

**Interpretation:**
- Remote workers experience more eye strain, likely from screen time without breaks.
- Hybrid and onsite workers report more back pain, which could be linked to workstation setups, commuting posture, or inconsistent ergonomics.

---

**Insights:**

Physical health issues show **clear patterns** linked to how and where people work — they're not evenly distributed.

- **Remote workers** face elevated risks of **eye strain and fatigue**, consistent with prolonged screen exposure and reduced movement throughout the day.
- **Hybrid and onsite employees** report more **back and neck pain**, reflecting inconsistent ergonomic setups, long hours at fixed desks, or commuting-related strain.
- **Education professionals** stand out with high rates of **shoulder pain**, possibly linked to frequent standing, lifting, or multitasking in dynamic classrooms.

These findings underscore the need for **targeted ergonomic strategies**, such as:
- Ergonomic equipment subsidies for hybrid and remote workers  
- Screen-time management tools or break reminders for remote teams  
- Task-specific posture and movement training for educators and operational staff

> By aligning interventions with the **unique physical demands of each role**, organizations can reduce pain-related absenteeism, improve comfort, and enhance productivity.

### Q4. What role does social isolation play in burnout and mental health?

**Objective**

To understand whether **social isolation** influences the likelihood of reporting burnout or other mental health conditions. This helps highlight the **emotional impact of disconnected work environments** and informs policies that prioritize connection and support.

---

**Data Cleaning & Processing**

- Removed all rows where `Mental_Health_Status` was `"None"`, since these do not contribute to meaningful mental health analysis.
- Used `str.split('; ')` and `explode()` on `Mental_Health_Status` to handle multi-condition responses.
- Focused the comparison on two key columns:
  - `Social_Isolation_Score` (1–10 scale)
  - `Burnout_Level` or individual `Mental_Health_Status` entries

```python
# CLEANING
mh_isolation = df[df["Mental_Health_Status"] != "None"].copy()
mh_isolation["Mental_Health_Status"] = mh_isolation["Mental_Health_Status"].str.split("; ")
mh_isolation = mh_isolation.explode("Mental_Health_Status")
```

---

**Data Preparation**

We used the `Social_Isolation_Score` (rated 1–10 by each employee) to compare against two outcomes:

- **Burnout_Level** (Low, Medium, High)
- **Mental_Health_Status** (multi-label: Anxiety, Depression, etc.)

---

**Step A: Social Isolation Score by Burnout Level**

We examined how the frequency of burnout levels changes across different levels of social isolation.

```python
burnout_pivot = df.pivot_table(
    index="Social_Isolation_Score",
    columns="Burnout_Level",
    aggfunc="size",
    fill_value=0
)
plt.figure(figsize=(8, 6))
sns.heatmap(burnout_pivot, annot=True, fmt="d", cmap="YlOrRd")
plt.title("Burnout Level by Social Isolation Score")
plt.xlabel("Burnout Level")
plt.ylabel("Social Isolation Score")
plt.tight_layout()
plt.show()
````

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20level%20by%20social%20isolation%20score.png)

**Key Observations:**

- High burnout cases increase consistently with higher isolation scores
- At isolation scores 8–10, High Burnout becomes the dominant category
- Low burnout is most common at isolation scores 1–3, then drops sharply

This pattern suggests a strong positive correlation between isolation and burnout severity.

---

**Step B: Social Isolation Score by Mental Health Condition**

```python
mh_pivot = mh_df.pivot_table(
    index="Social_Isolation_Score",
    columns="Mental_Health_Status",
    aggfunc="size",
    fill_value=0
)

plt.figure(figsize=(12, 6))
sns.heatmap(mh_pivot, annot=True, fmt="d", cmap="BuPu")
plt.title("Mental Health Issues by Social Isolation Score")
plt.xlabel("Mental Health Issue")
plt.ylabel("Social Isolation Score")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Mental%20Health%20Issues%20by%20Social%20Isolation%20score.png)

| Mental Health Condition | Avg. Social Isolation Score |
|--------------------------|-----------------------------|
| PTSD                     | 2.85                        |
| Depression               | 2.78                        |
| Anxiety                  | 2.70                        |
| ADHD                     | 2.64                        |
| Stress Disorder          | 2.63                        |
| Burnout                  | 2.52                        |


**Insights:**
The pivot table shows a clear rise in high burnout levels as isolation scores increase — especially from score 7 upwards. While average isolation scores are not extremely high overall, conditions like PTSD, Depression, and Anxiety consistently show higher isolation averages than burnout alone. This suggests that isolation is a stronger emotional trigger for deep mental distress than it is for everyday burnout — though both are impacted.

**Conclusion**
Social isolation appears to be modestly related to burnout, but its stronger emotional impact is seen in more severe mental health challenges.
Individuals experiencing PTSD and depression reported the highest isolation levels — suggesting that loneliness and disconnection are critical emotional risk factors that go beyond burnout.

These findings highlight the importance of fostering emotional connection, team belonging, and proactive outreach, especially for those at risk of deeper mental health strain.

### Q5. Do salary and region influence employee well-being and burnout levels?

**Objective**

To assess whether **salary** and **geographic region** are linked to differences in **burnout**, **mental health**, and **social isolation**. This helps uncover whether economic or cultural environments play a role in workplace well-being.

---

**Step A: Burnout Level by Salary Range**

```python
burnout_salary = df[df["Mental_Health_Status"] == "Burnout"].groupby(["Salary_Range", "Burnout_Level"]).size().reset_index(name="Count")

plt.figure(figsize=(10, 6))
sns.barplot(data=burnout_salary, x="Salary_Range", y="Count", hue="Burnout_Level", palette="magma")
plt.title("Burnout Levels by Salary Range")
plt.xlabel("Salary Range")
plt.ylabel("Number of Burnout Cases")
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20level%20by%20salary%20range%20.png)

| Salary Range   | High Burnout | Medium Burnout | Low Burnout | Total |
|----------------|--------------|----------------|-------------|--------|
| <$40K          | 36           | 41             | 28          | 105    |
| $40K–$60K      | 34           | 47             | 33          | 114    |
| $60K–$80K      | 18           | 34             | 26          | 78     |
| $80K–$100K     | 11           | 18             | 20          | 49     |
| $100K+         | 9            | 10             | 14          | 33     |

**Insight:** Lower-income groups (especially <$60K) show substantially higher burnout, particularly in the high and medium categories. Burnout rates drop noticeably at higher salary levels.

---

**Step B: Social Isolation Score by Region**
```python
isolation_region = df.groupby("Region")["Social_Isolation_Score"].mean().reset_index().sort_values("Social_Isolation_Score", ascending=False)

plt.figure(figsize=(10, 5))
sns.barplot(data=isolation_region, x="Region", y="Social_Isolation_Score", palette="Blues_r")
plt.title("Average Social Isolation Score by Region")
plt.ylabel("Avg. Social Isolation")
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Social%20Isolation%20score%20by%20region.png)

| Region        | Avg. Social Isolation Score |
|---------------|-----------------------------|
| South America | 3.01                        |
| Asia          | 2.88                        |
| North America | 2.72                        |
| Europe        | 2.55                        |
| Africa        | 2.50                        |


**Insight:** South America and Asia show the highest average isolation scores. This may reflect infrastructure challenges or fewer internal support systems.

---

**Step C: Mental Health Conditions by Salary Range**

```python
mh_salary = df[df["Mental_Health_Status"] != "None"].copy()
mh_salary["Mental_Health_Status"] = mh_salary["Mental_Health_Status"].str.split("; ")
mh_salary = mh_salary.explode("Mental_Health_Status")

mh_salary_summary = mh_salary.groupby("Salary_Range")["Mental_Health_Status"].value_counts().unstack().fillna(0)

plt.figure(figsize=(12, 6))
sns.barplot(data=mh_salary, x="Salary_Range", y="Count", hue="Mental_Health_Status", palette="Spectral")
plt.title("Mental Health Conditions by Salary Range")
plt.xlabel("Salary Range")
plt.ylabel("Number of Employees")
plt.legend(title="Mental Health Status", bbox_to_anchor=(1.05, 1), loc="upper left")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Mental%20Health%20conditions%20by%20Salary%20range%20.png)

| Salary Range | Anxiety | Burnout | Depression | PTSD |
|--------------|---------|---------|------------|------|
| <$40K        | 62      | 66      | 43         | 39   |
| $40K–$60K    | 58      | 61      | 41         | 33   |
| $60K–$80K    | 34      | 35      | 22         | 19   |
| $80K–$100K   | 19      | 22      | 15         | 9    |
| $100K+       | 14      | 16      | 8          | 5    |


**Insight:** All mental health conditions are most prevalent in the <$60K brackets, especially burnout and anxiety. Mental health challenges decrease as salary increases — highlighting the protective power of financial stability.

**Conclusion**
Employees in lower salary bands and in regions with higher isolation scores (like South America and Asia) face higher risks of burnout and mental health issues. Meanwhile, higher earners ($80K+) report far fewer issues, and regions like Europe and Africa show relatively lower social isolation.

These patterns suggest that economic strain and regional context are significant drivers of employee well-being.

> 💡 Key Findings: Salary & Region Impact
>
> - 🌍 **South America** has the highest isolation and high burnout proportion
> - 💰 **Burnout drops** significantly in employees earning **$80K+**
> - 😰 **Anxiety, depression, and PTSD** are most common in the **<$60K income group**
> - 🧭 Regional culture and salary may shape access to support, flexibility, and well-being

### Q6. How does work-life balance correlate with burnout and mental health?

**Objective**

To explore how **work-life balance** affects two key outcomes:
- **Burnout Level** (Low, Medium, High)
- **Mental Health Status** (Anxiety, Depression, Burnout, etc.)

This helps evaluate whether perceived balance between work and life is a protective factor against emotional exhaustion and mental health decline.

---

**Data Cleaning & Preparation**

- Used the column `Work_Life_Balance_Score` (assumed to range from 1–10).
- Converted mental health status to individual rows using `explode()`.
- Grouped both burnout and mental health conditions by **balance score ranges**.

---

**Step A: Burnout Level by Work-Life Balance Score**

```python
wlb_burnout = df[df["Mental_Health_Status"] == "Burnout"].copy()
wlb_burnout["WLB_Category"] = pd.cut(
    wlb_burnout["Work_Life_Balance_Score"],
    bins=[0, 3, 6, 10],
    labels=["Poor", "Moderate", "Good"]
)

burnout_wlb_summary = wlb_burnout.groupby(["WLB_Category", "Burnout_Level"]).size().reset_index(name="Count")

# Plot
sns.barplot(data=burnout_wlb_summary, x="WLB_Category", y="Count", hue="Burnout_Level", palette="Spectral")
plt.title("Burnout Level by Work-Life Balance")
plt.xlabel("Work-Life Balance")
plt.ylabel("Number of Burnout Cases")
plt.tight_layout()
plt.show()
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/Burnout%20levels%20by%20work-life-balance.png)

| Work-Life Balance | High Burnout | Medium Burnout | Low Burnout | Total |
|-------------------|--------------|----------------|-------------|--------|
| Poor              | 41           | 51             | 20          | 112    |
| Moderate          | 34           | 49             | 33          | 116    |
| Good              | 16           | 24             | 33          | 73     |

**Insight:** Employees with poor work-life balance reported the highest number of high burnout cases (41), while those with good balance showed a clear shift toward low burnout.

---

**Step B: Mental Health Status by Work-Life Balance Score**
```python
mh_wlb = df[df["Mental_Health_Status"] != "None"].copy()
mh_wlb["Mental_Health_Status"] = mh_wlb["Mental_Health_Status"].str.split("; ")
mh_wlb = mh_wlb.explode("Mental_Health_Status")

mh_wlb["WLB_Category"] = pd.cut(
    mh_wlb["Work_Life_Balance_Score"],
    bins=[0, 3, 6, 10],
    labels=["Poor", "Moderate", "Good"]
)

mh_wlb_summary = mh_wlb.groupby(["WLB_Category", "Mental_Health_Status"]).size().reset_index(name="Count")
```

![](https://github.com/Ujunwajohn01/Post-Pandemic-Remote-Work-Health-Impact-2025/blob/main/mental%20health%20issues%20by%20work-life%20balance.png)

| Work-Life Balance | Top Mental Health Issues         | Most Reported Issue | Count |
|-------------------|----------------------------------|----------------------|--------|
| Poor              | Burnout, Anxiety, Depression      | Burnout              | 53     |
| Moderate          | Burnout, Anxiety, Depression      | Burnout              | 49     |
| Good              | Anxiety, ADHD, Burnout            | Anxiety              | 24     |


**Insight:** As work-life balance improves, the frequency of burnout and depression decreases, while milder issues like anxiety remain more stable. This suggests strong balance may reduce severity, but not eliminate stress entirely.

**Interpretation**
Employees with poor work-life balance are significantly more likely to report high burnout and serious conditions like depression and burnout. By contrast, those with good balance tend to report fewer severe issues and more manageable stress symptoms like anxiety or ADHD. This confirms that work-life balance plays a protective role in mental health and emotional exhaustion.

## Recommendations

Based on the insights uncovered in this project, the following data-driven recommendations are proposed to improve employee well-being:


**1. Prioritize Mental Health in Hybrid and Onsite Models**
- Burnout and depression were most commonly reported among **hybrid and onsite** workers.
- Employers should invest in:
  - **Onsite wellness programs**
  - Regular **mental health check-ins**
  - Quiet or decompression zones in physical offices


**2. Address Burnout in the 26–35 Age Group & Long Work Hours**
- Employees aged **26–35** working **46–60 hours/week** reported the **highest burnout rates**.
- Solutions:
  - Implement workload management and **time-off policies**
  - Monitor hours via self-reporting or scheduling software
  - Create coaching programs for early-career employees


**3. Improve Work-Life Balance to Reduce Mental Health Strain**
- **High burnout (41 cases)** and **depression** were most common in employees with **poor WLB scores**.
- Encourage:
  - **Flexible scheduling** and autonomy
  - Clear separation of working and non-working hours
  - Training for managers on respecting work-life boundaries


**4. Consider Regional and Salary-Based Support Disparities**
- **South America and Asia** showed higher isolation scores and burnout.
- Lower-income employees (earning **<$60K**) had the **highest mental health challenges**.
- Recommendations:
  - Tailor interventions to **regional culture & digital access**
  - Provide mental health support that's **cost-free and confidential**
  - Include **stipends or resources** to improve remote work environments


**5. Combat Physical Health Issues with Ergonomic Solutions**
- **Back pain** and **eye strain** were the most common issues.
- Solutions:
  - Subsidize ergonomic chairs, monitors, and lighting
  - Provide education on posture and movement
  - Encourage **breaks and eye-rest intervals** in all work arrangements


**6. Tackle Social Isolation — Especially in Mental Health-Sensitive Roles**
- **High burnout** was concentrated in employees with **high isolation scores (8–10)**.
- **PTSD and depression** also had the **highest average isolation ratings**.
- Interventions:
  - Create **virtual peer groups or buddy systems**
  - Include **structured social time** in remote meetings
  - Train managers to spot signs of isolation and intervene early


## Conclusion

This project provides a comprehensive view of how remote and hybrid work environments impact **mental and physical health**, **burnout**, and **employee well-being** across demographics, regions, and industries.

**Key Takeaways:**
- **Burnout** is most prevalent in:
  - **Younger professionals**
  - Those with **poor work-life balance**
  - Employees working **long hours**
  - Lower-income and **onsite or hybrid roles**

- **Mental health issues** like depression, anxiety, and PTSD correlate more with:
  - **Isolation**
  - **Economic vulnerability**
  - **Lack of autonomy**

- **Physical complaints** such as back pain and eye strain are widespread, especially in **technology-heavy roles**, and vary by work model.

### Final Thought:
> A data-informed approach to wellness shows that **employee health is multi-dimensional** — shaped by workload, flexibility, salary, connection, and role design.
>  
> Organizations that invest in **customized, inclusive, and proactive well-being strategies** will benefit not just from healthier employees, but also from **improved retention, productivity, and culture**.

## Contact







