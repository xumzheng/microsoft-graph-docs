---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SetOrderPostRequestBody();
$newAssignmentOrder = new AssignmentOrder();
$newAssignmentOrder.setOrder(['City', 'extension_GUID_ShoeSize', ]);


$requestBody.setNewAssignmentOrder($newAssignmentOrder);


$graphServiceClient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignments().setOrder().post($requestBody);


```