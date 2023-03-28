---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new User();
$onPremisesExtensionAttributes = new OnPremisesExtensionAttributes();
$onPremisesExtensionAttributes->setExtensionAttribute1('skypeId.adeleVance');

$OnPremisesExtensionAttributes->setExtensionAttribute13(null);


$requestBody->setOnPremisesExtensionAttributes($onPremisesExtensionAttributes);


$requestResult = $graphServiceClient->usersById('user-id')->patch($requestBody);


```