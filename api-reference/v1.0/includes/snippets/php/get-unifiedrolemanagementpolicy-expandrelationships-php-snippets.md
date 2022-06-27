---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UnifiedRoleManagementPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters();
$queryParameters->expand = 'effectiveRules,rules';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->policies()->roleManagementPoliciesById('unifiedRoleManagementPolicy-id')->get($requestConfiguration);


```