---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();


$requestRequestBody->setDisplayName('My Class Team');
$requestRequestBody->setDescription('My Class Team’s Description');
$requestRequestBodyAdditionalData = [
	"template@odata.bind" => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teams()->post($requestRequestBody);


```