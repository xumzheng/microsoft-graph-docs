---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivatePostRequestBody()
subjectsUser1 = User()
subjectsUser1.setId('8cdf25a8-c9d2-423e-a03d-3f39f03c3e97')


subjectsArray []= subjectsUser1;
subjectsUser2 = User()
subjectsUser2.setId('ea09ac2e-77e3-4134-85f2-25ccf3c33387')


subjectsArray []= subjectsUser2;
request_body.setSubjects(subjectsArray)




await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').identityGovernanceactivate.post(request_body)


```