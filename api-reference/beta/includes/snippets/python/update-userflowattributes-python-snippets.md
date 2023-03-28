---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityUserFlowAttribute();
$requestBody->setDescription('Your new hobby');



$requestResult = $graphServiceClient->identity()->userFlowAttributesById('identityUserFlowAttribute-id')->patch($requestBody);


```