---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchemaPostRequestBody();


$requestRequestBodyAdditionalData = [
	"baseType" => 'microsoft.graph.externalItem',
	"properties" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->schema()->post($requestRequestBody);


```