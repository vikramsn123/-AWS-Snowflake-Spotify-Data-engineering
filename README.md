# Spotify Data Engineering End-to-End Project (AWS + Snowflake)
This project aimed to build a comprehensive end-to-end data engineering pipeline using AWS services. The primary focus was on understanding core services such as Lambda, S3, Athena, and CloudWatch, with an exploration of third-party integration into Snowflake using Snowpipe.

# Architecture Diagram
![image](https://github.com/user-attachments/assets/8c7a4300-b59b-443e-a761-e72f34b06c9f)

# Implementation Steps
1. Spotify API Integration: Utilized Python Jupyter notebooks for data analysis and segregation into three tables: artist, album, and songs.
![image](https://github.com/user-attachments/assets/b12c4f95-5aee-4b13-bea6-a1c781556bde)
2. AWS Lambda for Extraction: Deployed extraction code on AWS Lambda to fetch data directly from the Spotify API to an S3 bucket.
![image](https://github.com/user-attachments/assets/efb8107a-13af-49bd-936d-dd0477119d1b)
3. CloudWatch Trigger: Configured AWS CloudWatch triggers to execute the extraction process automatically every minute.
4. Transformation Function: Implemented a Lambda function for data transformation, automating the loading of transformed data to an S3 location using S3 event-based triggers.
![image](https://github.com/user-attachments/assets/4bf849e0-3b37-4d8c-bf12-93d61991ac6b)
5. File Organization on S3: Ensured proper organization of files on S3 for efficient data management.
![image](https://github.com/user-attachments/assets/cc14f909-61f5-4227-83b6-b4a5c2fb4237)
6.Glue and Athena Integration: Built analytics tables on data files using AWS Glue and Athena for interactive querying.
![image](https://github.com/user-attachments/assets/e5f45f8e-05e8-4dda-bc38-b21df89d1e01)
7.Integration with Snowflake: Explored third-party storage service integration by integrating S3 and Snowflake through Snowpipe.
![image](https://github.com/user-attachments/assets/ee9588fd-0706-4fd3-8ebe-12ca8eead02d)

# Results and Learnings
The project aims to provide end-to-end data engineering using AWS and Snowflake. This project has been a significant learning curve, particularly in handling JSON data formats. The majority of the data ingestion and transformation was accomplished during the initial data analysis and data transformation stages. Exploring AWS services like Lambda has provided valuable insights into the advantages of serverless computing.

The implementation of event triggering for automating pipelines, leveraging AWS IAM roles for robust security practices, and organizing data files in S3 to enhance the understanding of process flows. These aspects stand out as highlights of this project.

# Future Enhancements
As part of future enhancements, I plan to explore the integration of data visualization tools such as Amazon QuickSight and Power BI with the data warehouse. This addition will further enrich the analytical capabilities of the project.









