---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AppliesToRequestBuilderGetRequestConfiguration();

$queryParameters = new AppliesToRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,appId,displayName,createdDateTime';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->policies()->appManagementPoliciesById('appManagementPolicy-id')->appliesTo()->get($requestConfiguration);


```