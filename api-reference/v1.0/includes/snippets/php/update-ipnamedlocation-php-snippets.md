---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NamedLocation();


$requestRequestBody->setDisplayName('Untrusted named location with only IPv4 address');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.ipNamedLocation',
	"isTrusted" => False,
	"ipRanges" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->conditionalAccess()->namedLocationsById('namedLocation-id')->patch($requestRequestBody);


```