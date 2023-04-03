---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityUserFlowAttributeAssignment();
requestBody.setUserInputType(IdentityUserFlowAttributeInputType('textbox'));



result = awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id').patch(requestBody);


```