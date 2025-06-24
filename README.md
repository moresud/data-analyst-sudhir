Descriptive Analysis	2
Project Description:	2
Project Title:	2
Objective:	2
Dataset:	2
Methodology:	3
Tools and Technologies:	5
Deliverables:	5
AWS Deployment and Service Models	5
AWS Cost Analysis	9
AWS Global infrastructure	13
AWS IAM	15
AWS VPC	17
AWS Lambda	19
AWS EBS	20



Descriptive Analysis 
Project Description: 
Descriptive Analysis of Course Completion Patterns
This project focuses on analyzing student course completion patterns to help improve retention and learning outcomes. By conducting descriptive analysis, the project aims to identify key variables influencing completion rates and offer insights that guide academic support and curriculum design.
Project Title: Understanding Course Completion Patterns in Academic Programs
Objective: The primary goal of this project is to conduct a descriptive analysis of course completion data across multiple academic programs. This analysis aims to summarize completion trends, uncover gaps in student performance, and provide actionable insights that support curriculum improvement, workload balancing, and student engagement strategies.

Dataset: 
The dataset includes academic records for various programs and contains the following key attributes:
•	StudentID – Unique identifier for each student
•	CourseID – Course enrollment identifier
•	FacultyID – Responsible faculty member for the course
•	CompletionRate – Percentage of students completing the course
•	CompletionDate – Date of course completion
•	EnrollmentStatus – Indicates whether students enrolled, dropped, or completed
•	ProgramName – Degree or diploma program
•	GPA – Student performance metric
•	PaymentMethod – Indicates tuition funding method
•	RetentionStatus – Tracks continued engagement post-course

Methodology:
1 – Data Collection and Preparation:
•	Uploaded structured academic datasets to Amazon S3 for secure cloud storage.
•	Used AWS Glue DataBrew and Excel to profile and clean datasets.
•	Filled missing values with standardized placeholders (e.g., “NA”) and corrected data types.
•	Created relationships between parks and facilities (in your earlier example) or between courses and student/faculty data.
•	Identified and grouped data inconsistencies and standardized naming formats.
•	Ensured classification of data sensitivity for future compliance (public, internal, confidential).
2 – Descriptive Statistics:
•	Calculated average course completion rate across programs (24% baseline).
•	Evaluated course load and completion ratio by faculty and program.
•	Measured transaction frequency (enrollment) by course, program, and retention status.
•	Aggregated GPA and analyzed its correlation with course completion.
3 – Data Visualization:
•	Built bar charts showing average completion per program and faculty.
•	Created pie charts to represent student retention vs. dropout trends.
•	Designed line graphs to visualize time-based completion trends.
•	Used matrix-style diagrams to correlate GPA with course outcomes.
4 – Student Segmentation:
•	Segmented students based on GPA and frequency of enrollment.
•	Categorized students into high-performing, at-risk, and average-performance groups.
•	Analyzed behavioral trends across segments to identify intervention opportunities.
Insights and Findings:
•	Courses with low faculty-to-student ratios had significantly better completion rates.
•	Completion dropped during summer sessions and increased during fall.
•	Digital payment users showed slightly higher retention than those on cash-based plans.
•	Students with high GPA (>3.5) were more likely to complete courses across multiple programs.
•	Curriculum gaps and outdated content were common dropout triggers (as per fishbone diagram).
Recommendations:
•	Redesign orientation for new students to increase early engagement.
•	Balance teaching workloads to avoid burnout and improve course delivery.
•	Update curricula in low-completion programs based on trend insights.
•	Create targeted support plans for low-GPA or low-attendance segments.
•	Implement real-time data dashboards for faculty to monitor student progress.

Tools and Technologies:
•	Excel, Python (Pandas) – For data wrangling and descriptive stats
•	AWS S3, AWS Glue DataBrew – For data storage, profiling, and transformation
•	Power BI/Tableau – For building visual dashboards and communicating insights
Deliverables:
•	A cleaned and transformed dataset ready for reporting and deeper analysis
•	Visual dashboards representing course performance, student segmentation, and faculty metrics
•	A comprehensive report documenting methodology, findings, and strategic recommendations
This project provides actionable insight into student behavior and academic performance, enabling educators and administrators to optimize course design, improve retention strategies, and ensure equitable learning experiences across academic programs.

AWS Deployment and Service Models 
The three screenshots collectively demonstrate how course registration datasets are handled across various computing models (Traditional vs. Cloud), cloud deployment models (Private, Public, Hybrid, Multi-Cloud), and cloud service models (IaaS, PaaS, SaaS). The first diagram compares traditional and cloud computing by showing improvements in dataset location, access, and privacy. In the traditional model, data is externally stored and less flexible in access, while the cloud model leverages AWS infrastructure with secured access roles and encryption compliance for enhanced privacy and centralized control.

The second and third screenshot deepen the analysis by breaking down deployment and service model approaches. In the deployment models, the Private Cloud offers restricted access within the UCW network, while Public Cloud and Multi-Cloud expand access globally through federated credentials and varying privacy levels. In contrast, Hybrid Cloud provides a blend of shared control between on-premise and cloud environments. The service models (IaaS, PaaS, SaaS) focus on responsibility layers—where IaaS users manage OS and security, PaaS offers platform-level management, and SaaS provides fully managed solutions by the provider. These visuals effectively illustrate how cloud evolution enhances control, security, and flexibility in managing academic datasets.
    
AWS Cost Analysis 
The case study titled "Total Cost of Ownership – Delaware North" highlights how a large enterprise with 200+ locations and $3 billion in revenue optimized its IT operations by migrating to AWS. The organization faced challenges such as the need for rapid deployment of new solutions and frequent hardware upgrades. Their criteria for a new infrastructure included handling all workloads, reducing costs, and eliminating repetitive tasks like patching. To meet these needs, Delaware North shifted its on-premises data center to AWS, moving nearly all applications and eliminating 90% of its servers using reserved EC2 instances.
As a result, the company achieved notable gains including resource optimization, faster time-to-market, and improved operational efficiency. Additionally, other supporting visuals in the assignment showcase cost estimations for various academic operations like data profiling, data analysis, and data storage using AWS. These estimates provide a practical understanding of how different AWS services contribute to the overall cost-effectiveness and scalability of modern data infrastructure.

    


The following case study outlines the selection of the Developer Support Plan for the Academic Department. Since the academic team is focused on early-stage application development and testing, this support plan is ideal as it provides access to AWS technical resources, best practices, and expert guidance, perfect for experimenting with cloud-based solutions or running student labs efficiently. 
 

AWS Global infrastructure 
This screenshot compares three AWS infrastructure components—Regional Edge Cache, Edge Location, and Region—based on dataset location, access, and privacy. Regional Edge Caches, such as in Vancouver, BC, store publicly cached content for faster delivery, with read-only access and no sensitive data. Edge Locations like Seattle, WA, distribute CDN content geographically with limited access and short-term data transit. AWS Regions, such as Oregon, are used for storing sensitive and restricted data like logs or backups and are governed by IAM-controlled access for full operational control.

  

AWS IAM 
This module outlines the shared responsibility model between UCW and AWS for EC2 services and summarizes the successful completion of the IAM lab module. In the EC2 shared responsibility table, UCW is accountable for managing EC2 instances, including OS-level configurations, security patches, application environments, and ensuring the security and compliance of course-related datasets. AWS, in contrast, is responsible for maintaining the underlying EC2 infrastructure, managing the virtualization platform, and ensuring the durability and availability of storage services. This division allows UCW to focus on operational-level tasks while relying on AWS for core infrastructure stability and performance.
Additionally, the lab module on IAM (Identity and Access Management) was successfully completed, achieving a perfect score of 40/40. Tasks included adding users to specific support and admin groups, logging in with each user, and validating permission boundaries by attempting to stop EC2 instances. The activity demonstrated a practical understanding of IAM policy implementation, user group management, and permission-based access control in an AWS environment. This hands-on experience reinforces critical cloud governance skills essential for secure and scalable cloud operations.
   
AWS VPC
This lab focused on building a secure VPC environment by creating public and private subnets, setting up a NAT gateway, and launching an EC2 instance with proper routing and security group configurations. Tasks such as VPC creation, subnet setup, security group configuration, and EC2 deployment were completed successfully, earning full marks. However, the subnet route table association task received zero, likely due to a missing or incorrect configuration linking subnets to appropriate route tables. Despite this, the EC2 instance was accessible via the internet, indicating that key network components were functioning properly. Total score achieved: 25/30.
 

 
AWS Lambda 
In this AWS Lambda lab, I successfully created a Lambda function triggered by an Amazon EventBridge event to stop an EC2 instance on a scheduled basis. The activity involved setting up a scheduled expression, assigning appropriate IAM roles, and configuring the function to interact with the EC2 service securely. All four tasks—function creation, scheduling, configuration, and instance shutdown—were completed flawlessly, earning a perfect score of 20/20. This lab demonstrated automation capabilities in AWS, emphasizing event-driven computing and serverless execution.

 

 
AWS EBS
In Lab 4, focused on Amazon Elastic Block Store (EBS), I successfully created and attached an EBS volume to an EC2 instance and also created a snapshot, scoring 15 out of 25. While the initial setup tasks were completed correctly, I was unable to complete the steps involving mounting the volume and restoring the snapshot. Despite this, the lab provided valuable hands-on experience with AWS storage services and deepened my understanding of EBS functionalities, particularly in managing persistent storage and backup operations in cloud environments.
 

 

