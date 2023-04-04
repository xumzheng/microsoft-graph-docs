---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ActivatePostRequestBody()
subjectsUser1 = User()
subjectsUser1.setId('df744d9e-2148-4922-88a8-633896c1e929')


subjectsArray []= subjectsUser1;
request_body.setSubjects(subjectsArray)




await client.identityGovernance.lifecycleWorkflows.workflowsById('workflow-id').identityGovernanceactivate.post(request_body)


```