---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MembersRequestBuilderGetRequestConfiguration();

$queryParameters = new MembersRequestBuilderGetQueryParameters();
$queryParameters->filter = 'roles/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->members()->get($requestConfiguration);


```