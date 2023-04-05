---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(true)



result = await client.identityGovernance.lifecycleWorkflows.workflowsById('workflow-id').patch(request_body)


```