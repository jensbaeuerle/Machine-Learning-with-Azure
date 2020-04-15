# Setup Machine Learning Service

## **1. Workspace:**
* ### Create Workspace:
* ### Delete Workspace:
* ### Connect to Workspace:

# Connecting to an existing Azure Machine Learning Workspace

#Method 1 - with a configuration file (.json)
from azureml.core import Workspace
ws = Workspace.from_config()

#Method 2 - use the get method to connect
from azureml.core import Workspace
ws = Workspace.get(name="myworkspace",
               subscription_id='<azure-subscription-id>',
               resource_group='myresourcegroup')


## **2. Experiment:**

   * ### Create/Get Experiment:

   # 2. Create or connect to an Experiment (If the experiment is not found in the workspace, a new experiment is created.)

        from azureml.core import Experiment
        experiment = Experiment(workspace=ws, name="movieReview")

   * ### List all Experiment:

   * ### **Run:**
        * ### List all runs from the Experiment:
            * ### **Models:**
                * ### List all Models from AutoML Run:
                * ### Register Model:
                * ### Import Model file:
                * ### Get specific model:
                * ### **Deploy registered Model:**

## **3. Enterprise security for Azure Machine Learning:**


   




| Field  | Description |
| ------------- | ------------- |
|**Workspace name**|	Enter a unique name that identifies your workspace. In this example, we use docs-ws. Names must be unique across the resource group. Use a name that's easy to recall and to differentiate from workspaces created by others.|
|**Subscription**|	Select the Azure subscription that you want to use.|
|**Resource group**|	Use an existing resource group in your subscription, or enter a name to create a new resource group. A resource group holds related resources for an Azure solution. In this example, we use docs-aml.|
|**Location**|	Select the location closest to your users and the data resources to create your workspace.|
|**Workspace edition**|	Select Enterprise. This tutorial requires the use of the Enterprise edition. The Enterprise edition is in preview and doesn't currently add any extra costs.|



