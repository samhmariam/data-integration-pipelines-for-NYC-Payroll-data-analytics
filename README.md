# Data Integration Pipelines for NYC Payroll Data Analytics

## Project Overview

The City of New York would like to develop a Data Analytics platform on Azure Synapse Analytics to accomplish two primary objectives:

Analyze how the City's financial resources are allocated and how much of the City's budget is being devoted to overtime.
Make the data available to the interested public to show how the City’s budget is being spent on salary and overtime pay for all municipal employees.

### Project Goal

The goal is to create high-quality data pipelines that are dynamic, can be automated, and monitored for efficient operation. At the high level the pipelines looks like below:

![Pipeline Overview](./images/pipeline-overview.png)

### Project Steps

#### Step 1. Prepare the Data Infrastructure

    1. Create the data lake and upload data

        ![Payroll Directory](/images/payroll-directory.png)
        ![Historical Directory](/images/history-files-directory.png)
    
    2. Create SQL Database

        ![SQL Tables](/images/sql-db-tables.png)
    
    3. Create a Synapse Analytics workspace and Azure Data Factory

        ![Synapse External Table](/images/synapse-external-tables.png)
    
#### Step 2: Create Linked Services

    1. Create a Linked Service for Azure Data Lake and SQL Database

        ![Linked Services](/images/linked-services.png)

#### Step 3: Create Datasets in Azure Data Factory

    1. Create the datasets

        ![Datafactory Datasets](/images/datasets-datafactory.png)
    
#### Step 4: Create Data Flows

    1. Create Dataflows

        ![Datafactory Dataflows](/images/dataflows-datafactory.png)
    
    2. Create Data Aggregation and Parameterization dataflow

        ![Aggregation](/images/aggregate_dataflow-df.png)

#### Step 5: Pipeline Creation

    1. Create Pipeline

        ![Pipeline](/images/pipeline.png)

    2. Trigger and Monitor Pipeline

        ![Pipeline run](/images/pipeline_successful_run.png)

    3. Verify Pipeline run artifacts

        ![Artifacts](/images/sqldb-summary-table-query.png)
        ![dirstaging](/images/dirstaging-directory-files.png)
        ![Synapse External](/images/synapse-external-table-query-result.png)
    


