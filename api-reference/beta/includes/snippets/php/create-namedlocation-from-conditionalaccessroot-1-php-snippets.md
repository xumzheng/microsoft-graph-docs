---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NamedLocation();


$requestRequestBody->setDisplayName('Untrusted IP named location');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.ipNamedLocation',
	"isTrusted" => False,
	"ipRanges" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->conditionalAccess()->namedLocations()->post($requestRequestBody);


```