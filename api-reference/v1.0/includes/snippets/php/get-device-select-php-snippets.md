---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DeviceRequestBuilderGetRequestConfiguration();

$queryParameters = new DeviceRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,extensionAttributes';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->devicesById('device-id')->get($requestConfiguration);


```