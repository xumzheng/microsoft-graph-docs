---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->deviceManagement()->virtualEndpoint()->onPremisesConnectionsById('cloudPcOnPremisesConnection-id')->get($requestConfiguration);


```