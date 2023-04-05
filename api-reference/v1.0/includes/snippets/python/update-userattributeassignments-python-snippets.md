---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttributeAssignment()
request_body.setUserInputType(IdentityUserFlowAttributeInputType('textbox'))



result = await client.identity.b2xUserFlowsby_id('b2xIdentityUserFlow-id').userAttributeAssignmentsby_id('identityUserFlowAttributeAssignment-id').patch(request_body)


```