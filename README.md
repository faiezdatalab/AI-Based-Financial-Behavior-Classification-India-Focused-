# AI-Based-Financial-Behavior-Classification

Live Dashboard: https://public.tableau.com/views/AI-poweredfinancialbehaviorclassification/Dashboard1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link

### Overview

This project aims to classify Indian individuals based on their financial behavior — identifying whether someone is a Saver, Balanced, or an Over-Spender using AI. It’s a smart, usable solution that helps users understand their financial health and enables businesses (banks, fintechs, policy makers) to segment customers for personalized financial products.

### Objective

To build a value-driven AI system that:
* Classifies people into spending behavior categories
* Provides key insights into what drives saving habits
* Offers a real-time dashboard to analyze financial trends across demographics

###  Data

Synthetic yet realistic data based on Indian financial patterns with:

* 1000+ user profiles
* Features like income, expenses, savings, EMI, credit card usage, city tier, dependents, and financial literacy score
* Custom-added Indian-specific columns:
* City_Tier, Dependents, Financial_Literacy_Score, EMI_Obligations, Income_Level

### Methodology

Phase 1: Data Enrichment
* Created meaningful Indian context features
* Labeled spending patterns based on Savings Rate thresholds

Phase 2: EDA + Insights
* Explored how city tier, income, and dependents affect savings
* Identified that higher income doesn't guarantee high savings
* Found minimal correlation between financial literacy and actual saving habits

Phase 3: Feature Engineering
* Created new features like Income_Level_Code and dummies for ML
* Scaled and encoded data for better learning

Phase 4: AI Modeling
* Used Random Forest Classifier for explainability and performance
* Achieved 100% accuracy on test data
* Identified Savings Rate, Savings, and Income as top drivers

Phase 5: Tableau Dashboard
Published a fully interactive dashboard with 4+ dynamic charts:
* Savings vs Dependents
* Financial Literacy vs Savings Rate
* Spending Pattern by Tier
* EMI Load by Pattern
* Income vs Savings

### Key Insights

* City Tier vs Savings: Tier-2 users saved more than Tier-1 or Tier-3
* Dependents Impact: More dependents → less savings (but not always)
* EMI Behavior: Over-spenders have higher EMI loads
* Income ≠ Savings: Some low-income users saved better than high-income ones

###  Business Value

* Can be used by fintechs, banks, loan companies to score users
* Helps individuals self-assess their financial habits via dashboards
* Encourages personalized financial planning based on behavioral profiles

### Tech Stack

* Python: pandas, seaborn, sklearn, matplotlib
* Machine Learning: Random Forest Classifier
* Dashboarding: Tableau Public
