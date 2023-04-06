---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttributeAssignment()
request_body.setUserInputType(IdentityUserFlowAttributeInputType('textbox'))


request_config = IdentityUserFlowAttributeAssignmentRequestBuilderPatchRequestConfiguration(
request_config = IdentityUserFlowAttributeAssignmentRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments_by_id('identityUserFlowAttributeAssignment-id').patch(request_body, headers=)


```