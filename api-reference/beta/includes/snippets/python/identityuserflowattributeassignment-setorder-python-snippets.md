---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetOrderPostRequestBody()
newAssignmentOrder = AssignmentOrder()
newAssignmentOrder.Order(['City', 'extension_GUID_ShoeSize', ])


request_body.newAssignmentOrder = newAssignmentOrder



await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments.setOrder.post(request_body = request_body)


```