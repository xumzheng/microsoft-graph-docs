---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ContentRequestBuilderGetRequestConfiguration();

$queryParameters = new ContentRequestBuilderGetQueryParameters();
$queryParameters->format = '%7Bformat%7D';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->drive()->itemsById('driveItem-id')->content()->get($requestConfiguration);


```