---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConnectorGroup();
$requestBody->setName('name-value');

$requestBody->setIsDefault(false);



$requestResult = $graphServiceClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->connectorGroups()->post($requestBody);


```