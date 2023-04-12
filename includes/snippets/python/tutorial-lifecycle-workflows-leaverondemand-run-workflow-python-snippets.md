---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivatePostRequestBody()
subjectsUser1 = User()
subjectsUser1.id = '8930f0c7-cdd7-4885-9260-3b4a8111de5c'


subjectsArray []= subjectsUser1;
request_body.subjects(subjectsArray)





await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').identityGovernanceactivate.post(request_body = request_body)


```