---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProvider();


$requestRequestBody->setName('Login with Amazon');
$requestRequestBody->setType('Amazon');
$requestRequestBody->setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8');
$requestRequestBody->setClientSecret('000000000000');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.identityProvider',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityProviders()->post($requestRequestBody);


```