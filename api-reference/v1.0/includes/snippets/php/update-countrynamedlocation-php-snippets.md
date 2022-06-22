---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NamedLocation();


$requestRequestBody->setDisplayName('Updated named location without unknown countries and regions');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.countryNamedLocation',
	"countriesAndRegions" =>  [
'CA','IN',	],
	"includeUnknownCountriesAndRegions" => False,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->conditionalAccess()->namedLocationsById('namedLocation-id')->patch($requestRequestBody);


```