---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TaskReportsRequestBuilderGetRequestConfiguration(
request_configuration = TaskReportsRequestBuilderGetRequestConfiguration(query_params=query_params = TaskReportsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedUsersCount","processingStatus","successfulUsersCount","totalUsersCount","unprocessedUsersCount","taskDefinition","taskProcessingResults"]

)
query_params = TaskReportsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedUsersCount","processingStatus","successfulUsersCount","totalUsersCount","unprocessedUsersCount","taskDefinition","taskProcessingResults"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').taskReports.get(request_configuration)


```