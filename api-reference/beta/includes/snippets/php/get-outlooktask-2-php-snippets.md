---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OutlookTaskRequestBuilderGetRequestConfiguration();

$headers = [
	"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->outlook()->tasksById('outlookTask-id')->get($requestConfiguration);


```