---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetOrderPostRequestBody()
newAssignmentOrder = AssignmentOrder()
newAssignmentOrder.setOrder(['City', 'extension_GUID_ShoeSize', ])


request_body.setNewAssignmentOrder($newAssignmentOrder)


await client.identity_b2cUserFlowsby_id('b2cIdentityUserFlow-id')_userAttributeAssignments_setOrder.post(request_body)


```