---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UserRequestBuilderGetRequestConfiguration();

$queryParameters = new UserRequestBuilderGetQueryParameters();
$queryParameters->select = 'customSecurityAttributes';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->usersById('user-id')->get($requestConfiguration);


```