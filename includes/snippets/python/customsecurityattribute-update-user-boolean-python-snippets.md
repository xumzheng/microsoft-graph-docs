---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new User();
$customSecurityAttributes = new CustomSecurityAttributeValue();
$additionalData = [
'Engineering' => $customSecurityAttributes = new Engineering();
$		customSecurityAttributes->set@odatatype('#Microsoft.DirectoryServices.CustomSecurityAttributeValue');

		$customSecurityAttributes->setCertification(false);


$customSecurityAttributes->setEngineering($engineering);

];
$customSecurityAttributes->setAdditionalData($additionalData);



$requestBody->setCustomSecurityAttributes($customSecurityAttributes);


$requestResult = $graphServiceClient->usersById('user-id')->patch($requestBody);


```