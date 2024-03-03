RETAIL_ANALYSIS_END_TO_END_PROJECT

The "Retail Data Analysis" is a comprehensive and automated retail analysis project that utilizes various technologies and tools to provide valuable insights into customer buying patterns and seasonal trends



✦ 
Created an AWS S3 bucket and uploaded raw files securely. Implemented roles and policies for secure access and user-specific operations. Snowflake (SQL)


✦
Implementing code in SQL for automatic data ingestion from client uploads

Developing linkage between a Cloud environment and Snowflake using Amazon AWS S3 buckets
Utilizing S3 buckets for storing and managing data files, using 'copy into' command for loading content from source to destination


✦
Loading data from AWS S3 bucket to Snowflake table with external stage concept

External stage concept in Snowflake is like inviting data by creating a 'stage' before copying it into table.
Ensure Snowflake warehouse is active, not suspended, to smoothly execute data ingestion process.


✦
Snowpipe enables continuous data ingestion for faster availability of data.

1) Data is loaded from files in micro batches, making it available to users within minutes.
2) Snowpipe automates the data loading process, eliminating the need for manual execution of copy statements.


✦
Copying data from AWS S3 bucket to Snowflake account with notification creation.

1) Notification channel created upon data copy for status updates.
2) Emphasis on security measures and client access control for S3 bucket.


✦
Creating buckets and folders in AWS S3

1) Buckets need access permission to be freely accessible
2) Folders are like rooms inside a bucket, using simple commands to create


✦
Creating tables in Snowflake for data ingestion
Need to create tables for campaign, campaign description, coupon redemption, coupon demography   

✦
Setting up storage integration between Snowflake and AWS S3 bucket.

1) In this project my first Step was to create an AWS account, set up an S3 bucket, and create folders for data storage.
2) Importance of maintaining consistency in folder naming for seamless data integration and avoid errors.


✦
Understanding S3 bucket actions and resources
Actions such as put, get, delete, and object version are provided by default
The resource in S3 bucket includes ARN (Amazon Resource Name) and access control for folders   



✦
Creating policies and roles in AWS for data analytics
Retail policies and return policies can be created in AWS for specific roles. Policies and roles in AWS are essential for controlling access and permissions for data analytics



✦
Creating IAM Role in AWS

1) Third-party can assume roles in AWS to perform actions on behalf of the client.
2) Multiple policies can be attached to one role or vice versa in AWS IAM roles.



✦
Setting up storage integration and role in AWS S3 bucket
Creating AWS role Arn and user Arn is essential for storage integration. Including the generated Arn in the role's trust relationship is crucial to avoid errors



✦
Creating a retail stage for data ingestion
Defining the S3 bucket URL and file format for data integration. Establishing a linkage for data ingestion with guests waiting at the stage




✦
Setting up event notifications for data updates
Creating event notifications for data ingestion in AWS S3 Bucket. Configuring notifications to trigger specific actions based on data updates



✦
Continuous data ingestion process from AWS S3 bucket to Snowflake
The data is queued and notifications are sent for each stage of the process. Snowflake copies the file into a queue and then loads it into the target table


✦
Auto data ingestion in S3 bucket with no data loss

Shared two files, one after the other
Auto ingest feature scans files without code execution



✦
Data ingestion and schema differences
Data from different sources may require different tables and columns due to schema differences. Secure and optimized code is essential to handle data ingestion and ensure data integrity.



✦
Uploading data into AWS S3 bucket and Snowflake database.
Importance of saving column order for data ingestion. Creating a Scenario of uploading data to the coupon and product tables and checking for data consistency.







