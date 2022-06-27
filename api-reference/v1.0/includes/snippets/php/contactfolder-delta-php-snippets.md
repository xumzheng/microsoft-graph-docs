---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$headers = [
	"Prefer" => "odata.maxpagesize=2",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->contactFolders()->delta()()->get($requestConfiguration);


```