# NBA Data Lake

NBA Data Lake is a project designed to build a scalable data lake for NBA data using AWS cloud services. This setup allows for efficient storage, cataloging, and querying of NBA statistics and analytics data. The project integrates Amazon S3, AWS Glue, and Amazon Athena to create a robust data infrastructure for data-driven insights.

## Features

- **Data Storage**: Leverages Amazon S3 to store raw and processed NBA data.
- **Data Cataloging**: Utilizes AWS Glue to create a database and table for schema management.
- **Data Querying**: Enables SQL-based querying with Amazon Athena.
- **Sample Data Upload**: Includes a sample dataset in JSON format for demonstration purposes.

## Prerequisites

### API Key
- Sign up for a free account at [SportsDataIO](https://sportsdata.io/).
- Retrieve your API key under the "Query String Parameters" section in the NBA category.
- Update the `setup_nba_data_lake.py` script with your API key.

### AWS Permissions
Ensure your AWS IAM user or role has the following permissions:
- **S3**: `s3:CreateBucket`, `s3:PutObject`, `s3:DeleteBucket`, `s3:ListBucket`
- **Glue**: `glue:CreateDatabase`, `glue:CreateTable`, `glue:DeleteDatabase`, `glue:DeleteTable`
- **Athena**: `athena:StartQueryExecution`, `athena:GetQueryResults`

## Setup Instructions

### Step 1: Launch AWS CloudShell
1. Log in to your AWS account.
2. Open CloudShell from the AWS Management Console.

### Step 2: Create the Script
1. In CloudShell, create a new Python file:
   ```bash
   nano setup_nba_data_lake.py
   ```
2. Copy the content of the `setup_nba_data_lake.py` script from this repository and paste it into the editor.
3. Add your SportsDataIO API key in the designated section of the script.

### Step 3: Run the Script
1. Save and exit the editor.
2. Execute the script:
   ```bash
   python3 setup_nba_data_lake.py
   ```
3. The script will create the necessary AWS resources, upload sample data, and complete the data lake setup.

## Learning Outcomes

By completing this project, you will:
- Learn to set up a data lake using AWS cloud services.
- Gain experience in securing AWS services with IAM policies.
- Understand how to integrate external APIs into cloud-based workflows.

## Future Enhancements

- Automate data ingestion with AWS Lambda.
- Add a data transformation layer using AWS Glue ETL.
- Build advanced visualizations with AWS QuickSight.
- Incorporate real-time data streaming using AWS Kinesis.

## Contributions

Contributions are welcome! Please fork this repository, make your changes, and submit a pull request for review.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
-**Name**: Carl Anthony Osborne
-**linkedIn**: https://www.linkedin.com/in/carlanthonyosborne/
-**Github**: https://github.com/ehrconsultantforhire
-**eMail**: app@ehrconsultantforhire.com

For questions or feedback, please open an issue in this repository.

