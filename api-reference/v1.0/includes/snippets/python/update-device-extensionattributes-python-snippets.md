---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Device();
$additionalData = [
'extensionAttributes' => $requestBody = new ExtensionAttributes();
$		requestBody->setExtensionAttribute1('BYOD-Device');


$requestBody->setExtensionAttributes($extensionAttributes);

];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->devicesById('device-id')->patch($requestBody);


```