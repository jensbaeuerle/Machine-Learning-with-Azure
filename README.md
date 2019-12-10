# Machine-Learning-with-Azure
Machine Learning with different Azure Services (e.g. PowerBI, Azure Designer, Automated Machine Learning (Interface), Machine Learning Service)

## Prerequisites

- Azure Subscription
- PowerBI Premium
- PowerBI Desktop

## Visualization with PowerBI

#### Answer the following questions:
- How many sales per year?
- How many sales in year 1990 per month?
- How many Stores?
- How many Sales per Store and the average prize?
- How many brands?
- Average prize for brands in month?

## Machine Learning with PowerBI

#### Tutorial:

- https://docs.microsoft.com/en-us/power-bi/service-tutorial-build-machine-learning-model

1. Create Workspace
2. Create Dataflow from data source
3. Add a Machine Learning model
4. Get PowerBI model validation report
5. Apply the model to a dataflow entity

## Setup Machine Learning Service

1. Create Machine Learning Service in Azure:
  - Search for "Machine Learning" in the Azure Portal
  - Click "Create"
    - Workspace Name: Name of the Workspace
    - Subscription: Subscription
    - Resource Group: Resource Group
    - Location: Location of the service
    - Workspace edition: Edition of the Workspace (use Enterprise)
    
2. Go to the Machine Learning Service:
  - Launch the new Azure Machine Learning studio
  
3. Connect Datastores:
  - Click in the Azure Machine Learning studio on "Datastores"
  - Click on "New datastore"
    - Datastore name: Name of the Datastore
    - Datastore type: type of the Datastore
    - Subscription ID: Subscription where the datastore is located
    - Server name / database name: Server name
    - Authentication type: Authentication type
    - User ID: User ID
    - Password: Password of the Datastore
    
4. Create datasets:
  - Dataset 1: weekly Sales 
    - Click on "Create dataset"
    - Select "From datastore"
      - SQL Query:
        - Select WeekStarting, sum(Quantity) as Quantity 
        - from dbo.Sales
        - GROUP BY CAST(WeekStarting AS DATE)
        
  - Dataset 2: All Sales data:
    - Click on "Create dataset"
    - Select "From datastore"
  
  
  
  
  
  
  
## Automated Machine Learning (Interface)
#### Tutorial:
- https://docs.microsoft.com/en-us/azure/machine-learning/service/tutorial-first-experiment-automated-ml

## Machine Learning Designer

## Machine Learning Service

- General


