---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AppRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AppRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'resourceId%20eq%208e881353-1735-45af-af21-ee1344582a4d';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->usersById('user-id')->appRoleAssignments()->get($requestConfiguration);


```