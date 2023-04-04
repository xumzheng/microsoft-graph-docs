---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TaskReportsRequestBuilderGetRequestConfiguration();

query_params = TaskReportsRequestBuilderGetQueryParameters;
query_params.select = ["id","failedUsersCount","processingStatus","successfulUsersCount","totalUsersCount","unprocessedUsersCount","taskDefinition","taskProcessingResults"];

request_config.queryParameters = query_params;


result = await client.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').taskReports().get(request_config);


```