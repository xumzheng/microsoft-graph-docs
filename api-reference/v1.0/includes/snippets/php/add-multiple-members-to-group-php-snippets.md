---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBodyAdditionalData = [
	"members@odata.bind" =>  [
'https://graph.microsoft.com/v1.0/directoryObjects/{id}','https://graph.microsoft.com/v1.0/directoryObjects/{id}','https://graph.microsoft.com/v1.0/directoryObjects/{id}',	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groupsById('group-id')->patch($requestRequestBody);


```