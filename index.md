## Project Portfolio

---
## Scalable Genomic Annotation Service System
### Cloud Computing & Software Engineering

During UChicago's <a href="https://mpcs-courses.cs.uchicago.edu/2024-25/autumn/courses/mpcs-51083-1">Cloud Computing course</a> in Autumn 2024, I developed the Genomics Annotation Service (GAS)—a scalable, fault-tolerant, and cost-effective system designed to efficiently manage asynchronous workflows in a distributed cloud environment. The architecture leverages Amazon S3 for storing input files, results, and logs, while DynamoDB ensures persistent storage of job metadata. To enhance scalability and reliability, I implemented asynchronous inter-process communication and serverless workflows for various system functions. 

I utilized Amazon SNS, SQS, and webhooks to enable decoupled communication between system components, allowing the web application to publish job requests asynchronously. This design ensured that each service could scale independently in a cost-effective manner. For data archival and restoration, I created serverless workflows using AWS Step Functions and Lambda that integrated with Stripe’s payment API, facilitating efficient lifecycle management between S3 and Glacier based on user tiers, including users' account data and uploaded files. To handle varying workloads, I implemented auto-scaling and load balancing for both the web servers and the annotators, ensuring seamless performance under dynamic conditions.

The Github repo for this project is private, but I've made the exported code available <a href="https://drive.google.com/file/d/1OJ5KSlXKvHIr8I5Tw-sYudv_NDYaP3Jb/view">here</a>.



<img src="images/gas.png"/>

---
## End-to-End Lambda Architecture for Ad Hoc Reporting on Large-Scale Uber Trip Data
### Data Modeling & Software Engineering
During a <a href="https://harris.uchicago.edu/academics/programs-degrees/courses/big-data-and-development-winter-2023">Big Data and Development course</a> for UChicago's MSc in Computational Analysis and Public Policy in Winter 2023, I coded and deployed a cloud-based <a href="https://docgpt.herokuapp.com/">medical AI chatbot</a> using OpenAI’s Completions and Embeddings API endpoints. I used prompt engineering and text embeddings drawn from a knowledge base of 257k doctor-patient dialogues to improve model response. I wrote an accompanying <a href="https://github.com/dustinmarshall/DocGPT/blob/main/research_design.pdf">research design</a> for a health intervention using the app. The application is fully open-source on <a href="https://github.com/dustinmarshall/DocGPT">GitHub</a>.

<img src="images/lambda.jpg"/>

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
## Predicting Gentrification using Tract-level Characteristics
### Data Visualization & Machine Learning Code Sample
During a Machine Learning course for UChicago's MSc in Computational Analysis and Public Policy in Spring 2022, my group used 2016 census tract data of neighborhood characteristics to predict a binary classification of a neighborhood’s gentrification status in 2019. The dataset contained 778 census tracts with 22 feature variables measuring socioeconomic status, educational attainment, criminal activity, pollution level, transportation equity and housing equity. The annalysis compared the F1-score performance of logistic regression, decision tree, random forest, and gradient-boosted decision tree models. The code and final report are available on <a href="https://github.com/dustinmarshall/predicting_gentrification_using-ML">GitHub</a>.

<img src="images/ml.jpg"/>

---
## Interactive Dashboard Mapping Parks and Underutilized Public Land
### Data Visualization & Geospatial Analysis Code Sample
During a Computer Science course for UChicago's MSc in Computational Analysis and Public Policy in Winter 2022, my group coded a data visualization interface in Dash. The interface serves as a tool for urban planners to identify neighborhoods with disproportionately few green spaces and many vacant lots to be considered for conversion. My contribution focused on collecting, cleaning, and wrangling the data on green spaces and vacant lots using the City of Chicago and Cook County's APIs. The code and written report are available on <a href="https://github.com/dustinmarshall/less-vacant-places-more-green-spaces">GitHub</a>.

<img src="images/dash.jpg"/>
