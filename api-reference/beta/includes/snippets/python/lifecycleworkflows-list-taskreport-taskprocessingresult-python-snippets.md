---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = TaskProcessingResultsRequestBuilderGetRequestConfiguration(
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').taskReports_by_id('taskReport-id').taskProcessingResults.get()


```