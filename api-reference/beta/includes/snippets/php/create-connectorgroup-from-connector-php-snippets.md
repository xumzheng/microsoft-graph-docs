---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->connectorsById('connector-id')->memberOf()->ref()->post($requestRequestBody);


```