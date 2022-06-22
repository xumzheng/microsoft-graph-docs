---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBodyAdditionalData = [
	"template@odata.bind" => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
	"group@odata.bind" => 'https://graph.microsoft.com/beta/groups(\'71392b2f-1765-406e-86af-5907d9bdb2ab\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```