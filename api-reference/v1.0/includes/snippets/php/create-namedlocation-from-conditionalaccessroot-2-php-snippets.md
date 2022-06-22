---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NamedLocation();


$requestRequestBody->setDisplayName('Named location with unknown countries and regions');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.countryNamedLocation',
	"countriesAndRegions" =>  [
'US','GB',	],
	"includeUnknownCountriesAndRegions" => True,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->conditionalAccess()->namedLocations()->post($requestRequestBody);


```