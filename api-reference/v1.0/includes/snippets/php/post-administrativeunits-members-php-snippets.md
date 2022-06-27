---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Ref();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/v1.0/groups/{id}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->directory()->administrativeUnitsById('administrativeUnit-id')->members()->ref()->post($requestRequestBody);


```