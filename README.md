### Vanguard A/B Testing Analysis


## 📌 Overview

This project analyzes the results of Vanguard's digital experience A/B test to evaluate whether a redesigned online process improved customer completion rates and overall user experience.

The experiment compared Vanguard's existing digital process (Control) with a redesigned experience (Test) that introduced updated navigation and user guidance. The goal was to determine whether the new design increased successful completions while reducing customer friction.

---

## 🎯 Objectives

We investigated the following key questions:

* Did the new design improve completion rates?
* Did the redesign reduce customer drop-offs?
* Did the new experience reduce user errors?
* Which process steps generated the most friction?
* Which customer segments benefited most from the redesign?
* Should Vanguard replace the existing design?

---

## 📊 Dataset

The analysis combines three datasets provided by Vanguard:
## 📊 Dataset

Source: Ironhack Data Analytics Bootcamp – Vanguard A/B Testing Case Study

Files Used:

* df_final_demo.txt
* df_final_experiment_clients.txt
* df_final_web_data_pt_1.txt
* df_final_web_data_pt_2.txt
* 
### Client Profiles

Contains customer demographic and account information.

Key variables:

* client_id
* clnt_age
* gendr
* clnt_tenure_yr
* num_accts
* bal

### Digital Footprints

Tracks customer interactions throughout the online process.

Key variables:

* visitor_id
* visit_id
* process_step
* date_time

### Experiment Roster

Identifies the experimental group assigned to each client.

Key variable:

* Variation (Control or Test)

---

## ⚙️ Tools Used

* Python (Pandas, NumPy)
* SciPy
* Jupyter Notebook
* Tableau Public
* GitHub

---

## 🧹 Data Cleaning and Preparation

Several preprocessing steps were performed:

* Merged all datasets using client_id
* Removed incomplete and irrelevant records
* Filtered observations to Control and Test groups only
* Created process-step sequencing
* Generated completion flags
* Created drop-off indicators
* Identified backtracking behavior
* Calculated repeat-step activity
* Created demographic groupings for age and tenure

---

## 📈 Key Performance Indicators (KPIs)

The following KPIs were used to evaluate the redesigned experience:

### ✅ Completion Rate

Percentage of users who successfully reached the confirmation step.

### 🚪 Drop-off Rate

Percentage of users who abandoned the process before completion.

### ⚠️ Error Rate

Percentage of sessions containing backward navigation (backtracking).

### 🔄 Repeat Step Rate

Percentage of users repeating one or more process steps.

### ✔️ Confirmation Repeat Rate

Percentage of users repeating the confirmation step.

---

## 📊 Key Findings

### Completion and Drop-Off Performance

* The Test design improved customer completion rates.
* The Test group experienced lower drop-off rates compared to the Control group.
* More users successfully progressed through the redesigned journey.

### User Friction

* Error rates increased in the Test group.
* Repeat-step behavior was more frequent in the redesigned experience.
* The Start and Confirm steps generated the highest levels of friction.

### Customer Segments

* Older clients (61+) achieved the highest completion rates.
* Longer-tenure customers adapted most successfully to the redesigned process.
* The redesign appeared to be most effective for experienced Vanguard clients.

---

## 🔍 Funnel Analysis

A funnel analysis was performed to examine customer progression through the process:

Start → Step 1 → Step 2 → Step 3 → Confirm

The largest user losses occurred during the early stages of the process, indicating opportunities for improving onboarding and navigation clarity.

---

## 🧪 Hypothesis Testing

Statistical testing was conducted to evaluate whether observed differences between Control and Test groups were significant.

Tests focused on:

* Completion rate differences
* Drop-off rate differences
* User behavior and process performance

Results supported the conclusion that the redesigned experience influenced customer behavior, although increased friction remains a concern.

---

## 📋 Business Recommendation

The redesigned experience shows potential by increasing successful completions and reducing abandonment.

However:

* Error rates increased
* Users repeated steps more frequently
* Friction remained concentrated at the Start and Confirm stages

### Recommendation

* Refine the onboarding experience
* Simplify confirmation screens
* Address identified friction points
* Conduct a follow-up experiment before full deployment

---

## 🧪 Workflow

1. Data exploration and business understanding
2. Data cleaning and dataset merging
3. Feature engineering and KPI creation
4. Exploratory data analysis
5. KPI comparison between Control and Test groups
6. Funnel analysis
7. Friction analysis
8. Demographic analysis
9. Hypothesis testing
10. Tableau dashboard and story creation
11. Business recommendations

---

## 🚀 Deliverables

* Jupyter Notebook
* Cleaned Dataset
* Tableau Public Story
* README
* Final Presentation

---

## 📌 Conclusion

The redesigned Vanguard experience improved completion rates and reduced customer abandonment. However, the increase in user errors and repeated actions indicates that usability issues remain.

The findings suggest that Vanguard should refine key friction points before fully replacing the existing design. A revised version of the redesign should be tested in a future experiment to validate improvements.

---

## 🔗 Links


**Tableau Story:** https://public.tableau.com/views/Vanguard_AB_Testing_Final/Story1

**Repository:** https://github.com/romsx111/ab-customer-experience-project

**Presentation:** https://docs.google.com/presentation/d/1zzjiazxC8J0jE3S6Q-fdAD6FLGj75Jq7/edit?usp=sharing&ouid=101958444504053526965&rtpof=true&sd=true

**Trello Board: https://trello.com/invite/b/6a0f5b51972f22bcc9308dc0/ATTI5f33e2253782e0189b199b2ac87c5c0749493753/a-b-experiment
