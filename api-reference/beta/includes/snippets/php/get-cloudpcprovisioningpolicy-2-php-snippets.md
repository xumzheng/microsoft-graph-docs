---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPcProvisioningPolicyRequestBuilderGetQueryParameters();
$queryParameters->expand = 'assignments';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->deviceManagement()->virtualEndpoint()->provisioningPoliciesById('cloudPcProvisioningPolicy-id')->get($requestConfiguration);


```