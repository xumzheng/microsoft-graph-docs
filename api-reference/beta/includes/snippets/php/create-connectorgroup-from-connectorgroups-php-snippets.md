---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConnectorGroup();


$requestRequestBody->setName('name-value');
$requestRequestBody->setIsDefault(False);
$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->connectorGroups()->post($requestRequestBody);


```