---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BundlesPostRequestBody();


$requestRequestBodyAdditionalData = [
	"name" => 'My Day at the Beach',
	"@microsoft.graph.conflictBehavior" => 'rename',
	"children" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->drive()->bundles()->post($requestRequestBody);


```