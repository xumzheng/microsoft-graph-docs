---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ActivatePostRequestBody()
subjectsUser1 = User()
subjectsUser1.setId('8930f0c7-cdd7-4885-9260-3b4a8111de5c')


subjectsArray []= subjectsUser1;
request_body.setSubjects(subjectsArray)




await client.identityGovernance_lifecycleWorkflows_workflowsby_id('workflow-id')_identityGovernanceactivate.post(request_body)


```