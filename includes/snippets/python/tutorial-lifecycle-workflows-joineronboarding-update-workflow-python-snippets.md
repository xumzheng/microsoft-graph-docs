---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(true)


request_config = WorkflowRequestBuilderPatchRequestConfiguration(
request_config = WorkflowRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').patch(request_body, headers=)


```