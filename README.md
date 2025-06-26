# elevate-labs-project
# company : Elevate labs
# internship :  Data Analytics

** Explanation :
🔹 STEP 1: Dataset Collection
Objective: Obtain Shark Tank India or US datasets (CSV/Excel format).

Action:
  Download datasets from sources like Kaggle or GitHub:
  Search for “Shark Tank India Dataset CSV”
  Example fields to look for: Startup Name, Industry, Ask Amount, Invested Amount, Equity Given, Founders, Stage, Sharks, Deal, Country, etc.
  
🔹 STEP 2: Data Cleaning & Preparation (Using Python or Excel)
   Tools: Python (Pandas) or Excel

Action Items:
    Remove nulls, duplicates.
    Standardize domain names (e.g., “Tech”, “Technology”, “IT” → “Technology”).
Extract:
      Industry/domain
      Investment amount
      Equity given
      Founder count/gender
      Funding stage (Seed, Series A, etc.)
      Investor (Shark) names
      
Python Example:
      import pandas as pd
      df = pd.read_csv("sharktank_data.csv")
      df.drop_duplicates(inplace=True)
      df.dropna(subset=["Startup Name", "Industry", "Invested Amount"], inplace=True)
      df["Industry"] = df["Industry"].str.strip().str.lower()

🔹 STEP 3: Data Analysis
3.1. Industry-wise Investment Trends
      Total invested amount per industry
      Number of startups funded per domain
      Average ticket size per sector

3.2. Founder Profile Analysis
    Solo vs co-founders
    Gender analysis (if available)
    Industry vs founder type success
3.3. Funding Stage Success
  Which stages got most deals?
  Average investment per stage
  Deal conversion rate (ask vs got)

3.4. Shark/Investor Analysis
     Most active investors
     Sectors favored by each Shark
     Co-investment patterns
🔹 STEP 4: Data Visualization in Tableau
  Bar Chart: Total Investment by Industry
  Pie Chart: Deal Distribution by Funding Stage
  Line Chart: Investment Trend Over Seasons (if multiple seasons)
  Heatmap: Industry vs Shark Participation
  Stacked Bar: Founder type (solo/co-founder/gender) vs Deal Success
🔹 STEP 5: Report & Summary
Insights:
  Top 5 industries by funding
  Most successful founder profiles
  Best-performing funding stages
  Sharks with highest investments
  Visual Dashboard Screenshots
✅ Deliverables
    Cleaned dataset (CSV/Excel)
    Tableau .twbx or .pdf dashboard
    PDF Report with visuals + summary
