---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/v1.0/directoryObjects/{id}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->owners()->ref()->post($requestRequestBody);


```