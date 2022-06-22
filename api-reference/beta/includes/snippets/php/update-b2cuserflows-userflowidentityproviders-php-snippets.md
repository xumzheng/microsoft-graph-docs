---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase-idPatchRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/identity/identityProviders/{id}',
	"@odata.type" => '#microsoft.graph.identityProvider',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->userFlowIdentityProvidersById('identityProviderBase-id')->patch($requestRequestBody);


```