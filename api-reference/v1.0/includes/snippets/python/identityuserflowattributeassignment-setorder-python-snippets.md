---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SetOrderPostRequestBody();
newAssignmentOrder = AssignmentOrder();
newAssignmentOrder.setOrder(['City', 'extension_GUID_ShoeSize', ]);


requestBody.setNewAssignmentOrder($newAssignmentOrder);


awaitclient.identity().b2xUserFlowsById('b2xIdentityUserFlow-id').userAttributeAssignments().setOrder().post(requestBody);


```