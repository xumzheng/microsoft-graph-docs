---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DataSource();


$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.ediscovery.siteSource',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->sourceCollectionsById('sourceCollection-id')->additionalSources()->post($requestRequestBody);


```