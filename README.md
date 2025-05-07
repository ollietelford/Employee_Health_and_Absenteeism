# Employee Health and Absenteeism
## 🎯 Objective
The HR department provided the following brief:
1. Identify the healthiest employees to receive a shared bonus of £1,000
2. Allocate a wage increase to non-smokers using a £983,221 budget provided by the insurance company
3. Create a dashboard to help HR better understand absenteeism trends, based on an approved wireframe

-----
## 🔍 Dataset Overview
The dataset included information on absenteeism (such as reasons and hours missed), employee health data (including BMI, smoker and drinker status), and personal details like number of children, pets, and education level.

The data was loaded into SQL from CSV files to conduct exploratory data analysis (EDA) and to calculate the first two parts of the brief. This also allowed unnecessary fields to be removed before loading the cleaned data into Power BI for dashboard creation.

-----
### 1. Healthiest Employees
The healthiest employees were determined to be those who dont drink or smoke and have a healhty BMI (18.5-25), however as this still yielded too many records it was further narrowed down to exclude those who were absent more than average - giving a 111 employees to share the £1000 bonus or £9 each.

-----
### 2. Wage Increase for Non-smokers
To determine the healthiest employees, the criteria used were:
- Non-smokers
- Non-drinkers
- Healthy BMI (18.5–25)
This initially returned too many results, so the selection was further refined by excluding employees whose absenteeism was above average. This yielded 111 employees, who would share the £1,000 bonus — equating to approximately £9 each.

There are 686 non-smokers eligible for a wage increase. Based on an average of 2,080 work hours per year (40 hours × 52 weeks), the £983,221 budget allows for a:
- £0.68 hourly increase, or
- £1,414.40 annual bonus per employee

Calculation:
- Total hours = 2,080 × 686 = 1,426,880 hours
- Hourly increase = £983,221 ÷ 1,426,880 = £0.68/hour
- Annual increase = £0.68 × 2,080 = £1,414.40/year

-----
### 3. Creating the Dashbord
Additional categorical fields were created in SQL for BMI range and seasonal absenteeism to better analyze trends. The cleaned and enriched data was then imported into Power BI, where a dashboard was developed following the approved wireframe.
The dashboard includes:
- Key KPIs and summary narrative
- Employee breakdowns and categories
- Absence trends over time
- Absence reasons and comparisons

📊 Key Insights
- Average hours absent per employee: 6.92
- Total absences: 740
- Total hours lost: 5,124

Most absences were due to planned medical appointments (GP, dental, physiotherapy), while unplanned medical absences were less frequent. A total of 76 absences were marked as either unknown or unjustified.

Absenteeism decreases over the week, from an average of 9.2 hours on Monday to 5.1 hours on Friday. This weekly trend is generally consistent across all seasons. The months with the highest absenteeism rates were March, May, July, and December.The dashboard shows avergae hourse absent of 6.92 over 740 total absences which amounts to 5 124 total hours absent. The majority of these absences were due to planned medical procedures such as GP or dental appointments as well as physiotherapy while unplanned medical absences accounted for fewer total absences and unknown or unjustified absences accounted for 76 of the 740 total. Absences generally decrease as the week progresses from an average of 9.2 on Monday 5.1 on Friday, this trend can be genrally seen across all seaons while March, May, July and December show the highest rates of absenteeism.

-----
This dataset was taken from: https://absentdata.com/data-analysis/where-to-find-data/
