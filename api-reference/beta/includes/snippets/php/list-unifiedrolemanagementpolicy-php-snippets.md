---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RoleManagementPoliciesRequestBuilderGetRequestConfiguration();

$queryParameters = new RoleManagementPoliciesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'scopeId%20eq%20\'/\'%20and%20scopeType%20eq%20\'DirectoryRole\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->policies()->roleManagementPolicies()->get($requestConfiguration);


```