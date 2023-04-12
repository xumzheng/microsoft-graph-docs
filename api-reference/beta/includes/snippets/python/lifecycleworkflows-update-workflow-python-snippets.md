---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.description = 'Configure new hire tasks for onboarding employees on their first day'

request_body.displayName = 'Australia Onboard new hire employee'

request_body.isEnabled = true

request_body.isSchedulingEnabled = false




result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').patch(request_body = request_body)


```