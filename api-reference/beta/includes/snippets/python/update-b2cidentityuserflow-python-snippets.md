---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new B2cIdentityUserFlow();
$requestBody.setIsLanguageCustomizationEnabled(true);

$requestBody.setDefaultLanguageTag('en');



$requestResult = $graphServiceClient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').patch($requestBody);


```