---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Place();


$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.room',
	"nickname" => 'Conf Room',
	"building" => '1',
	"label" => '100',
	"capacity" => 50,
	"isWheelChairAccessible" => False,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->placesById('place-id')->patch($requestRequestBody);


```