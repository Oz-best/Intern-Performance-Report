# Intern-Performance-Report
This report highlights performance gaps in the internship program: uneven grader workloads, lack of communication, and breaching the performance gaps.
# Intern-Performance-Report

**Introduction**: The goal of this project is to analyse intern performance data across different teams and identify meaningful insights that can support better decision making within the internship program. The business objectives includes:

1. Evaluate intern performance across different stacks.
2. Identify patterns in grading and submission behavior.
3. Assess consistency in evaluation across graders.
4. Provide actionable recommendations to improve intern outcomes and program efficiency. 


**Project Overview:** This analysis is designed to:
1. Improve decision making for internship management.
2. Identify high performing and struggling interns.
3. Highlight inefficiencies in grading or submission processes.
4. Support better coordination between teams and evaluation.
5. Enhance overall internship quality and learning outcomes.


**Dataset Overview:** The dataset is from Trueminds Innovation and it includes the following fields:
1. Intern number: Unique identifier for each intern
2. Grade: Performance score assigned.
3. Graded At: Date/time grading was completed.
4. Submitted At: Date/time deliverable was submitted.
5. Stack: Intern’s role (UI/UX, Fronted, Backend, etc).
6. Graded By: Evaluator responsible for grading


**Business Questions:** The analysis and presentation slide should aim to answer:
1. Which stacks are performing best or worst?
2. Are there delays between submission and grading?
3. Do certain graders grade more strictly or leniently?
4. Is there a relationship between submission timing and grades?
5. Are there inconsistencies in grading across teams?


**Data Cleaning and Preparation:** Data preparation was done in Python Jupernotebook and PowerBi. 
Pandas, Numpy, Matplotlib, Seaborn, and Scikit-learn where used for data cleaning and preparation in python jupyternotebook. The date columns in the dataset were stored as object/text. Later converted both to datetime format using pd.to_datetime() for time based analysis. Checked for nulls using .isnull().sum() and it showed that the dataset has no missing values. Outliers were detected in the grade column which made 0.7% of outliers. Winsorization (0.01) was used to minimize the outliers.


**Dashboard Link**

https://app.powerbi.com/groups/me/reports/1c364ea6-de53-474b-bd12-19587fdf3de9/ReportSection?experience=power-bi


**Dashboard Design and Insights:** The interactive dashboard in Power BI was designed to present insight clearly and efficiently. Key features and insight include: 
1. Grading Overview: Shows the total grades by high and low performing stack and day delayed by graders and stack.
2. Intern and Grader Activity: shows the time the interns submitted and the time the intern were graded, graded consistency across stack and the grader classification.


**Key Metrics:** Total Interns 565(high performace 83.5%, low performance 16.5%), Avg grade 7.23(min grade 3, max grade 10), Avg waiting days 18.48(on time grading 0.4%, late grading 99.6%), Total graders 10(lenient graders 30%, strict graders 70%).


**KEY INSIGHT**

**1. Grading Overview:** Other roles at 100% high performance and Backend closely at 97.5% are the best performing stack while Graphic Designer with only 59.5% high performance and 40.5% low performance which show that graphic designers are the low performing stack. UI/UX and Frontend have the highest intern count but mid-range performance at 84.5% and 82.0%. Anthony Osadolo takes 38days to grade Backend developers, 39days to grade Other roles, and 27days to grade Frontend developers. Bidemi Afolabi takes 32days to grade Backend developers, 26days to grade Other roles. Kolawale Temilade takes 22days to grade Frontend developers. Wisdom Izozoima takes 18days to grade Frontend developers, takes 17days to grade Social media managers, and 6days to grade Project managers. Gift Izuchukwu takes 17days to grade Frontend developers, takes 17days to grade Social media managers, and 11days to grade Project managers. Victoria Okono takes 13days to grade Social media managers, and takes an average of 9days to grade Project managers. Ibrahim Jalladeen takes 11days to grade Social media managers, takes 10days to grade UI/UX designers, and takes 11days to grade Project managers. Grace Henry takes 20days to grade Project managers, takes 13days to grade UI/UX designers, takes 10days to grade Social media managers, takes 7days to grade Other roles, and takes 6days to grade Graphic desingers. Boluwatife Kayode takes an average of 11days to grade UI/UX desingers. Super admin takes 7days to grade Frontend developer. The stacks with the highest delays are Backend developers(37days), followed by Other roles(24days) and Frontend develpers(23days). The graders with the highest number of stacks they are grading are Grace Henry(grading 5 stacks), Anthony Osadolo(grading 3 stacks), Wisdom Izozoima(grading 3 stacks), Gift Izuchukwu(grading 3 stacks) and Ibrahin Jalladeen(grading 3 stacks). This shows that there is no clear division of labor and this creates bottlenecks. This also shows that the Backend developers is the biggest pain point. It also shows that Anthony and Bidemi has the highest workload + highest delay. It also shows that 7 out of 10 graders handle 3+ different stacks. Context switching = delays.


**2. Intern and Grader Activity:** Dead Zone(1am - 8am, almost no submission). Active zone(9am - 11pm, this is when 80%+ of submissions comes in). Peak 11pm with 64 submissions. Interns are submitting late at night). Grader active hours(8am - 7pm, this matches when most grading happens). Peak grading(7pm with 42 graded. That's the busiest hour). Misalignment(submissions peak at 11pm, but grading peaks at 7pm. There's a 4-hours gap where submissions pile up overnight). 3 graders(Boluwatife(7.81), Ibrahim(8.38) and Kolawole(7.57)) are giving scores above the overall average. This could mean easier grading or better quality from their interns. Grading is consistent across stacks. All scores falls between 6 - 7.6. No stack is being graded way harder or easier than others. Difference is <1 point. Also late night submissions contributes to grading delays because graders' activity stops at 7pm while submissions peak at 11pm. This creates an overnight backlog of hours. Also the long days of delay can also breach communication between the graders and the interns which can make some of the intern lose interest in the internship program.


**Recommendations**

Based on insights, these are the suggested improvement:
1. Improve submission timelines and deadlines.
2. Provide additional support for underperforming stacks.
3. Improve communication between interns and graders
4. Introduce performance tracking dashboards.
5. There should be at most 2 graders for one stack.











