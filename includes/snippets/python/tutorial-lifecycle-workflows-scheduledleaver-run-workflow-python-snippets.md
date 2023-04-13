---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivatePostRequestBody()
subjects_user1 = User()
subjectsUser1.id = 'df744d9e-2148-4922-88a8-633896c1e929'


subjectsArray []= subjectsUser1;
request_body.subjects(subjectsArray)





await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').identityGovernanceactivate.post(request_body = request_body)


```