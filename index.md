## Project Portfolio

---
## Scalable Genomic Annotation Service System with AWS
### Cloud Computing & Software Engineering
<img src="images/gas.png"/>

During UChicago's <a href="https://mpcs-courses.cs.uchicago.edu/2024-25/autumn/courses/mpcs-51083-1">Cloud Computing course</a> in Autumn 2024, I developed the Genomics Annotation Service (GAS)—a scalable, fault-tolerant, and cost-effective system designed to efficiently manage asynchronous workflows in a distributed cloud environment. The architecture leverages Amazon S3 for storing input files, results, and logs, while DynamoDB ensures persistent storage of job metadata. To enhance scalability and reliability, I implemented asynchronous inter-process communication and serverless workflows for various system functions. 

I utilized Amazon SNS, SQS, and <a href="https://www.redhat.com/en/topics/automation/what-is-a-webhook">webhooks</a> to enable decoupled communication between system components, allowing the web application to publish job requests asynchronously. This design ensured that each service could scale independently in a cost-effective manner. For data archival and restoration, I created serverless workflows using AWS Step Functions and Lambda that integrated with <a href="https://docs.stripe.com/api">Stripe’s payment API</a>, facilitating efficient lifecycle management between S3 and Glacier based on user tiers, including users' account data and uploaded files. To handle varying workloads, I implemented auto-scaling and load balancing for both the web servers and the annotators, ensuring seamless performance under dynamic conditions.

The Github repo for this project is private, but I've made the exported code available <a href="https://drive.google.com/file/d/1OJ5KSlXKvHIr8I5Tw-sYudv_NDYaP3Jb/view">here</a>.



---
## End-to-End Lambda Architecture for Ad Hoc Reporting on Large-Scale Uber Trip Data
### Data Modeling & Software Engineering
<img src="images/lambda.jpg"/>

This project implements a <a href="https://www.snowflake.com/guides/lambda-architecture/">Lambda Architecture</a> to analyze <a href="https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page">high-volume for-hire vehicle (HVFHV)</a> trips in New York City using Azure HDInsight Clusters. The architecture combines batch processing of large datasets with real-time analysis, providing hourly insights into key metrics of trip efficiency and pricing dynamics for major ride-sharing services. Metrics such as average price, wait time, trip duration, and costs related to tolls and congestion surcharges are analyzed and broken down by carrier, pickup location, dropoff location, and hour of the day. A Node.js web application serves as the front-end, enabling users to interact with the processed data and generate ad hoc reports.

The system is structured into three main layers:
1. **Batch Layer**: Processes historical data stored in **HDFS** and **Hive**, enabling comprehensive analysis of past trends.
2. **Serving Layer**: Combines batch views from **HBase** with incremental views to support efficient ad hoc querying.
3. **Speed Layer**: Handles real-time data processing using **Kafka** and **Spark Streaming**, ensuring up-to-date insights.

Data is sourced from <a href="https://data.cityofnewyork.us/Transportation/2022-High-Volume-FHV-Trip-Records/g6pj-fsah/about_data">the New York Open Data Portal</a>, with historical datasets bulk downloaded and real-time data fetched via the <a href="https://dev.socrata.com/foundry/data.cityofnewyork.us/g6pj-fsah">Socrata API</a>. This architecture delivers a scalable, fault-tolerant system that seamlessly integrates batch and real-time analytics, empowering users with actionable insights into New York City's ride-sharing ecosystem. The application is fully open-source on <a href="https://github.com/jycc-267/big-data-hvfhv-uber">GitHub</a>.



---
## Using Singular Value Decomposition to Detect Partisan Voting
### Machine Learning & Data Analysis Code Sample + Academic Writing Sample
During a <a href="https://willett.psd.uchicago.edu/teaching/mathematical-foundations-of-machine-learning-fall-2021/">Mathematical Foundations of Machine Learning course</a> in UChicago's Computer Science Department in Fall 2022, I co-authored an ML analysis of federal and state voting records. We used singular value decomposition and non-negative matrix factorization to detect partisanship in voting behavior, finding two clear voting blocs at both the national and state level that align with party affiliation. The <a href="https://github.com/dustinmarshall/detecting_partisan_voting_using_SVD/blob/main/detecting_partisanship_using_SVD.ipynb">code</a> and accompanying <a href="https://github.com/dustinmarshall/detecting_partisan_voting_using_SVD/blob/main/detecting_partisanship_using_SVD.pdf">academic paper</a> are available on GitHub.

<img src="images/svd.jpg"/>

---
## D3 Visualization for Vaccine Hesitency Chatbot Intervention 
### Data Visualization & Javascript Code Sample
During a Data Visualization course for UChicago's MSc in Computational Analysis and Public Policy in Fall 2022, I created a data vizialization in D3.js using the preliminary results of an ongoing <a href="https://osf.io/mgyxu/">chatbot intervention</a> to improve vaccine acceptance in Kenya and Nigeria with Prof. Molly Offer-Westort and DIL Director Leah Rosenzweig. The visualization is coded using the JavaScript library D3.js, which is used to produce dynamic, interactive data visualizations in web browsers. It includes a chloropleth map, grouped bar charts, and heatmaps. The code is available on <a href="https://github.com/dustinmarshall/data_visualization_for_policy_analysis/tree/main/final_project">GitHub</a>.

<img src="images/d3.jpg"/>

---
## Text Classification Model to Improve Grantee Discovery
### Machine Learning & Data Analysis Code Sample + Blog Writing Sample
During an internship with the Rockefeller Foundation's Data Science team in Summer 2022, I worked on a project mapping the non-profit space with natural language processing and machine learning. I built a subject classification model to classify their corpus of grant proposals to aid grantee discovery. The model is open-source on <a href="https://github.com/dustinmarshall/data_science_subject_classifier">GitHub</a> and a <a href="https://medium.com/mlearning-ai/using-nlp-to-improve-grantee-discovery-adc40f3833f">blog post</a> detailing the process was published on a popular machine learning blog on Medium.

<img src="images/nlp.jpg"/>

---
## Impact Evaluation of Covid-19 Precautions on Traffic Accidents
### Panel Data Analysis & Regression Discontinuity
<img src="images/trafficRD.jpg"/>

During a Machine Learning course for UChicago's MSc in Computational Analysis and Public Policy in Spring 2022, my group used 2016 census tract data of neighborhood characteristics to predict a binary classification of a neighborhood’s gentrification status in 2019. The dataset contained 778 census tracts with 22 feature variables measuring socioeconomic status, educational attainment, criminal activity, pollution level, transportation equity and housing equity. The annalysis compared the F1-score performance of logistic regression, decision tree, random forest, and gradient-boosted decision tree models. The code and final report are available on <a href="https://github.com/dustinmarshall/predicting_gentrification_using-ML">GitHub</a>.



---
## Interactive Dashboard Mapping Parks and Underutilized Public Land
### Data Visualization & Geospatial Analysis Code Sample
During a Computer Science course for UChicago's MSc in Computational Analysis and Public Policy in Winter 2022, my group coded a data visualization interface in Dash. The interface serves as a tool for urban planners to identify neighborhoods with disproportionately few green spaces and many vacant lots to be considered for conversion. My contribution focused on collecting, cleaning, and wrangling the data on green spaces and vacant lots using the City of Chicago and Cook County's APIs. The code and written report are available on <a href="https://github.com/dustinmarshall/less-vacant-places-more-green-spaces">GitHub</a>.

<img src="images/dash.jpg"/>
