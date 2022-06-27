---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalItem-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"acl" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->itemsById('externalItem-id')->put($requestRequestBody);


```