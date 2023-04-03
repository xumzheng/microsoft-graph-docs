---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ActivatePostRequestBody();
subjectsUser1 = User();
subjectsUser1.setId('8930f0c7-cdd7-4885-9260-3b4a8111de5c');


subjectsArray []= subjectsUser1;
requestBody.setSubjects(subjectsArray);




graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').identityGovernanceActivate().post(requestBody);


```