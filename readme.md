# ELT Using Azure Data Factory

This project scrapes data from the site [WillRobotsTakeMyJob](https://willrobotstakemyjob.com/) using Azure Virtual Machines. The scraped data consists of nine CSV files, each containing 100 data points per page. The data is injected into Azure Data Lake Storage Gen2, then concatenated and transformed into a Parquet file for efficient querying.

Transformations were performed in Azure Data Factory using Data Flow mapping and Spark pools so that the data is ready for analytics. The transformed data was then stored in a separate ADLS2 container. Finally, the processed data was imported into [Tableau](https://public.tableau.com/app/profile/anudeep.kolluri4281/viz/WillRobotsTakeMyJob_com/WillRobotsTakeMyJob) for visualizations.

---

## Architecture  
![Architecture Diagram](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/AI%20Occupation%20Systems%20Diagram.png)

## Screenshots  
- ![Pipeline](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/Pipeline.png)  
- ![Data Flow](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/DataFlow.png)  
- ![Visualization GIF](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/VizDemo.gif)

## Resources  
- **Dataset:** [occupations.csv](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/occupations.csv)  
- **Notebook (for testing):** [Analysis.ipynb](https://github.com/abhi-2699/Data-Factory-Project/blob/main/assets/Analysis.ipynb)  
- **Learning:** [Microsoft Learn DP-203](https://learn.microsoft.com/en-us/certifications/exams/dp-203/)

## Skills Used  
- Azure Data Factory  
- Azure Virtual Machines  
- Azure Data Lake Storage  
- PySpark  
- Azure Data Flow  
- Tableau  
- Python  
- SQL  
- Networking and Firewall  
