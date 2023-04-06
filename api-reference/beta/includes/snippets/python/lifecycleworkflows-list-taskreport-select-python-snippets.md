---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TaskReportsRequestBuilderGetRequestConfiguration(
request_config = TaskReportsRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","failedUsersCount","processingStatus","successfulUsersCount","totalUsersCount","unprocessedUsersCount","taskDefinition","taskProcessingResults"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').taskReports.get(request_config, headers=request_config)


```