---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBody->setDisplayName('My Sample Team');
$requestRequestBody->setDescription('My Sample Team’s Description');
$requestRequestBodyAdditionalData = [
	"template@odata.bind" => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```