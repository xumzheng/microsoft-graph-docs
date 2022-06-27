---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new FieldValueSet();


$requestRequestBodyAdditionalData = [
	"Color" => 'Fuchsia',
	"Quantity" => 934,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->sitesById('site-id')->listsById('list-id')->itemsById('listItem-id')->fields()->patch($requestRequestBody);


```