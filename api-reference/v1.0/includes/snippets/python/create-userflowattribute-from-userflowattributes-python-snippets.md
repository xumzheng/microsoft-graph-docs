---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityUserFlowAttribute();
$requestBody->setDisplayName('Hobby');

$requestBody->setDescription('Your hobby');

$requestBody->setDataType(new IdentityUserFlowAttributeDataType('string'));



$requestResult = $graphServiceClient->identity()->userFlowAttributes()->post($requestBody);


```