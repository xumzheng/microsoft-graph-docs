---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CloudPCRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPCRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->deviceManagement()->virtualEndpoint()->cloudPCsById('cloudPC-id')->get($requestConfiguration);


```