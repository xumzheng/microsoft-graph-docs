---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DriveItemRequestBuilderGetRequestConfiguration();

$queryParameters = new DriveItemRequestBuilderGetQueryParameters();
$queryParameters->expand = 'children';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sharesById('sharedDriveItem-id')->driveItem()->get($requestConfiguration);


```