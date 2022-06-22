---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase();


$requestRequestBody->setDisplayName('Sign in with Apple');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.appleManagedIdentityProvider',
	"developerId" => 'UBF8T346G9',
	"serviceId" => 'com.microsoft.rts.b2c.test.client',
	"keyId" => '99P6D879C4',
	"certificateData" => '******',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->identityProviders()->post($requestRequestBody);


```