# Versatus-GUIDE

## Step 1: Install the LASR CLI

To get started with the LASR CLI, you need to install it. Ensure that you have Python installed on your system (preferably version 3.6+).

You can install the CLI using pip:

```
pip install lasr
```
## Step 2: Initialize the LASR CLI

Once installed, initialize LASR by configuring the environment and setting up the necessary credentials.

```
lasr init
```
This command will guide you through configuring the following:

API Key: Set your API key for authentication.

Default Project: Select or create a default project.

## Step 3: Verify Installation

To ensure the installation was successful and the LASR CLI is working correctly, run the following:

```
lasr --version
```
This should return the version of LASR you have installed.

## Step 4: Create a New Project

To start using LASR, create a new project. You can do this with:

```
lasr create project <project_name>
```
Replace <project_name> with the desired name for your project.

Example:

```
lasr create project my_project
```
## Step 5: Add a Data Source

Next, you'll need to add a data source to your project. This is the data that LASR will process. The following command will allow you to add a new data source:

```
lasr add datasource <source_name> <path_to_data>
```
Example:

```
lasr add datasource customer_data ./data/customers.csv
```
This command will add the customers.csv file as the customer_data source.

## Step 6: Run Data Processing

Once the data source is added, you can run data processing on it. Use the process command to start:

```
lasr process <datasource_name>
```
Example:

```
lasr process customer_data
```
This command will start the data processing workflow for the customer_data source.

## Step 7: Check the Status

While the data is being processed, you can check the status of the process using the status command:

```
lasr status <datasource_name>
```
Example:

```
lasr status customer_data
```
This will show you the current status of the data processing.

## Step 8: View Processed Data

After processing is complete, you can view the results by using the view command:

```
lasr view <datasource_name>
```
Example:

```
lasr view customer_data
```
This will display the processed data output for the customer_data source.

## Step 9: Generate a Report

If you want to generate a report based on the processed data, you can do so with the following command:

```
lasr report generate <project_name>
```
Example:

```
lasr report generate my_project
```
This will create a detailed report for your project.

## Step 10: Cleanup Resources

After completing your work, you may want to clean up resources (such as data or models) associated with your project. Use the delete command:

```
lasr delete project <project_name>
```
Example:

```
lasr delete project my_project
```
This will delete all the data and resources associated with my_project.
