---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationContextClassReference();


$requestRequestBodyAdditionalData = [
	"value" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->conditionalAccess()->authenticationContextClassReferencesById('authenticationContextClassReference-id')->patch($requestRequestBody);


```