---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityUserFlowAttributeAssignment();
requestBody.setUserInputType(IdentityUserFlowAttributeInputType('textbox'));



result = await client.identity().b2xUserFlowsById('b2xIdentityUserFlow-id').userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id').patch(requestBody);


```