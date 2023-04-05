---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.setDescription('Configure new hire tasks for onboarding employees on their first day')

request_body.setDisplayName('Australia Onboard new hire employee')

request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(false)



result = await client.identityGovernance_lifecycleWorkflows_workflowsby_id('workflow-id').patch(request_body)


```