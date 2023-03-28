---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Language();
$additionalData = [
'id' => 'es-ES', 
'isEnabled' => true,
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->languagesById('userFlowLanguageConfiguration-id')->put($requestBody);


```