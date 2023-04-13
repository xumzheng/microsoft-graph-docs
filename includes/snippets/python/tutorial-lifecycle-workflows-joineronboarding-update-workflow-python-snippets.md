---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.is_enabled = True

request_body.is_scheduling_enabled = True




result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').patch(request_body = request_body)


```