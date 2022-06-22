---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.socialIdentityProvider',
	"clientSecret" => '1111111111111',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->identityProvidersById('identityProviderBase-id')->patch($requestRequestBody);


```