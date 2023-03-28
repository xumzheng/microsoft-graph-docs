---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ActivatePostRequestBody();
$subjectsUser1 = new User();
$subjectsUser1.setId('df744d9e-2148-4922-88a8-633896c1e929');


$subjectsArray []= $subjectsUser1;
$requestBody.setSubjects($subjectsArray);




$graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').identityGovernanceActivate().post($requestBody);


```