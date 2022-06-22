---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test',
	"@odata.type" => '#microsoft.graph.identityProvider',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userFlowIdentityProviders()->ref()->patch($requestRequestBody);


```