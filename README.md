# weather_project_aws-snowflake-dynamodb-s3
Unlock the power of AWS Data Engineering in our series, where we dive into DynamoDB, Snowflake, EventBridge, and AWS Lambda to build a dynamic real-time data pipeline. Learn how to connect a weather API, transfer data into DynamoDB, and effortlessly stream it to Snowflake using Snowpipe.

Created a weather API with an API key to fetch data using a Python script.
Set up an EventBridge schedule to trigger a Lambda function every hour.
The Lambda function retrieves data from the weather API and stores it in a DynamoDB table.
Inserting data into the DynamoDB table generates a DynamoDB stream.
A Lambda function processes this stream and loads the data into AWS S3.
Configured Snowpipe to send a notification via SQS to Snowflake.
Once notified, Snowflake ingests data from the S3 external stage.
