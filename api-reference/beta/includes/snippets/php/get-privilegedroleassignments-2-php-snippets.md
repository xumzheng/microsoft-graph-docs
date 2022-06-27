---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'isElevated%20eq%20true';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->privilegedRoleAssignments()->get($requestConfiguration);


```