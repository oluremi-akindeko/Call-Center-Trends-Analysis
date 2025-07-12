# Call Center Trends Analysis

<img width="1025" height="577" alt="image" src="https://github.com/user-attachments/assets/a666c2d5-7e40-4262-8a74-e0df21c198ec" />



# Introduction
This Power BI project focuses on analyzing call center data for Phone Now (*a fictional telecom company*) in order to track key performance metrics, optimize agent efficiency, and improve customer satisfaction score. By transforming raw data into an interactive dashboard, the project delivers clear insights into call volumes, resolved calls, agent performance, and actual customer satisfaction rating vs targetted rating which empower data-driven decision-making and operational improvement.
# Skills Demonstrated
- Data Cleaning
- Data modelling
- Data Visualization
- DAX measures
- Filters
- Critical Thinking
- Problem Solving
- Interpreting visuals to extract business insights
# Dashboard Goal
The stakeholders had requested that the dashboard show the following metrics:
- Overall customer satisfaction vs target
- Overall calls answered/abandoned
- Calls by month
- Calls by topic
- Average speed of answering calls
- Call center Agent’s performance quadrant
# Data Sourcing
After defining the problem statement, I sourced the dataset by downloading an Excel file from the Forage platform and imported it into Power BI. The dataset covered call center operations for the first quarter of 2021, specifically from January 1 to March 31. I performed data cleaning to ensure accuracy and consistency, followed by in-depth analysis and the development of interactive visualizations to address key business questions and uncover actionable insights.
# Data transformation/Cleaning
The dataset was initially not ready for analysis and required thorough cleaning and transformation before analysis. Using Power BI’s Power Query Editor, the data was efficiently prepared. Ensuring consistency, accuracy, and readiness for visualization.
## Applied data cleaning steps
- Changing Data Types
- Added conditional column for call status
![image](https://github.com/user-attachments/assets/4f8e1da2-96f3-4ed7-997c-d05b89c0fbc2)
The highlighted column represents the newly created column. You may also review the applied steps pane for a detailed breakdown of the transformation process.
- Reordered column
- Added conditional column for resolution status
![image](https://github.com/user-attachments/assets/0b544051-9743-4ed0-8bb2-72569db3b049)
- Replaced 'Pennding' to 'Unresolved' in the resolution status column
![image](https://github.com/user-attachments/assets/963ddb57-72da-49bb-8fec-02801d31cea1)
- Created a calendar table
![image](https://github.com/user-attachments/assets/6e2fcba4-c7fd-44fd-a3fc-f314f74af402)
This was done to enables robust and accurate time-based analysis and custom date filtering.
- Developed eight calculated measures using DAX to deliver key metrics aligned with stakeholder requirements.
# Data Modeling
I developed a data model that establishes a many-to-one relationship between the main call center data table and a calendar table, enabling efficient date-based filtering and advanced time intelligence analysis.
![image](https://github.com/user-attachments/assets/f0b7dff1-34da-48c0-a0d5-222b4e0d4c79)
# Analysis and Visualization
This section presents key insights derived from the call center dataset using interactive Power BI visuals. By leveraging charts, tables, slicers and KPIs, the analysis highlights performance trends, agent productivity, call handling efficiency, and customer satisfaction metrics. These visuals are designed to support data-driven decision-making and provide a clear view of operational strengths and areas for improvement.
## Overall customer satisfaction vs target
The gauge visual displays the average customer satisfaction score, which currently stands at 3.40 out of a possible 5.00. This is measured against a predefined target score of 4.00, indicating that while customer sentiment is generally positive, it falls below the desired benchmark.
The visual effectively highlights the performance gap, signaling a need for targeted improvements in customer service delivery, agent responsiveness, or issue resolution processes to enhance overall satisfaction and meet the set goal.

![image](https://github.com/user-attachments/assets/e9f85748-c77e-4b50-b2b2-2a54cd25539a)
## Overall calls answered/abandoned
The dashboard shows that 81.08% of calls were answered, while 18.92% were abandoned. This indicates a need to reduce missed calls. Additionally, 89.94% of answered calls were resolved, reflecting strong service performance, though 10.06% remain unresolved and may require further attention.

![image](https://github.com/user-attachments/assets/eb37031e-b89d-43ca-86fe-3a1b0e6a503a)
## Calls by month
The month of January recorded the highest call volume, with a total of 1,772 calls—exceeding February and March by 156 and 160 calls, respectively. It also had the highest number of answered calls (1,455), surpassing February by 157 and March by 154. Similarly, resolved calls peaked in January at 1,311, compared to 1,161 in February and 1,174 in March.
This trend suggests that January, being the start of a new year, is typically a busier period for customer interactions.

![image](https://github.com/user-attachments/assets/da291f36-5363-4811-bd96-c1d20c619e38)
## Calls by topic
Out of a total of 5,000 calls received during the calendar year, the highest volume of complaints was related to streaming, accounting for 1,022 calls (20.44%). This suggests that streaming issues were the most common concern among customers. In contrast, contract-related issues recorded the lowest volume, with 976 calls (19.52%), indicating it was the least reported topic during the period.

![image](https://github.com/user-attachments/assets/b1fd7565-0ab8-4c41-802d-62a04169a747)
## Average speed of answering calls
The average speed of answering calls stands at 67.52 seconds, which reflects the typical wait time customers experience before being connected to an agent. While this may be acceptable in some cases, it could also contribute to the 18.92% call abandonment rate observed.

![image](https://github.com/user-attachments/assets/c76c72e6-d914-4955-8947-06a078542be2)
## Call center Agent’s performance quadrant
The performance matrix highlights individual agent metrics across key areas during the calendar year. Jim led in both call volume and resolution, handling 536 calls (13.22%) and resolving 485 (13.30%)—the highest among all agents. In contrast, Stewart recorded the lowest in both categories, with 477 calls answered (11.77%) and 424 resolved (11.63%).
While Jim excelled in volume, Martha achieved the highest customer satisfaction score at 3.47, outperforming Joe, who scored the lowest at 3.33. In terms of responsiveness, Becky was the fastest, averaging 65.33 seconds per call, while Joe had the slowest response time at 70.99 seconds.
This quadrant reveals varying strengths across agents, offering actionable insights for targeted training and performance optimization.

![image](https://github.com/user-attachments/assets/01302901-42e7-436f-8d17-d73f5b732591)
# Conclusion and Recommendation
These are five actionable suggestions for the Management Team based on the call center data analysis to improve KPIs and boost customer satisfaction:
- **Reduce Call Abandonment through Improved Staffing:**
The 18.92% abandonment rate suggests delays in answering. Align staffing levels with peak call periods and consider implementing callback options or queue announcements to reduce drop-offs.
- **Enhance Agent Training on Streaming Issues:**
Since streaming accounts for the highest complaint volume (20.44%), targeted training and knowledge base improvements can help agents resolve these issues faster and more accurately.
- **Set and Monitor SLA for Average Response Time:**
With an average answer time of 67.52 seconds, setting a service level target (e.g., answer within 45 seconds) and monitoring adherence can reduce wait times and abandonment.
- **Leverage High Performers for Peer Coaching:**
Agents like Jim and Martha show strength in volume and customer satisfaction, respectively. Use them as internal benchmarks or mentors to support underperforming team members like Joe and Stewart.
- **Incentivize Customer-Centric Behavior:**
Reward agents not just for call volumes but also for resolution rates, satisfaction scores, and responsiveness. This can foster a more balanced, customer-focused performance culture.

![image](https://github.com/user-attachments/assets/8197948d-379e-42bb-b373-eafd7e659449)

Thanks for following through.








