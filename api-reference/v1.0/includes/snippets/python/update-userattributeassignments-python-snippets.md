---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttributeAssignment()
request_body.UserInputType(IdentityUserFlowAttributeInputType('textbox'))




result = await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').userAttributeAssignments_by_id('identityUserFlowAttributeAssignment-id').patch(request_body = request_body)


```