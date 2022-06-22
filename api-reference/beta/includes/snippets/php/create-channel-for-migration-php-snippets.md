---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Channel();


$requestRequestBody->setDisplayName('Import_150958_99z');
$requestRequestBody->setDescription('Import_150958_99z');
$requestRequestBody->setCreatedDateTime(new DateTime("2020-03-14T11:22:17.067Z"));
$requestRequestBodyAdditionalData = [
	"@microsoft.graph.channelCreationMode" => 'migration',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->channels()->post($requestRequestBody);


```