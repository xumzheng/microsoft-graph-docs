---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProviderBase();


$requestRequestBody->setDisplayName('Login with Amazon');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.socialIdentityProvider',
	"identityProviderType" => 'Amazon',
	"clientId" => '56433757-cadd-4135-8431-2c9e3fd68ae8',
	"clientSecret" => '000000000000',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->identityProviders()->post($requestRequestBody);


```