---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = WorkflowVersionRequestBuilderGetRequestConfiguration(
request_configuration = WorkflowVersionRequestBuilderGetRequestConfiguration(query_params=query_params = WorkflowVersionRequestBuilderGetQueryParameters()
query_params['select'] = ["category","displayName","versionNumber","executionConditions"]
query_params['expand'] = ["tasks"]

)
query_params = WorkflowVersionRequestBuilderGetQueryParameters()
query_params['select'] = ["category","displayName","versionNumber","executionConditions"]
query_params['expand'] = ["tasks"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').versions_by_id('workflowVersion-versionNumber').get(request_configuration)


```