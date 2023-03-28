---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityUserFlowAttributeAssignment();
$requestBody.setUserInputType(new IdentityUserFlowAttributeInputType('textbox'));



$requestResult = $graphServiceClient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id').patch($requestBody);


```