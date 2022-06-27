---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters->select = 'allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->groupsById('group-id')->get($requestConfiguration);


```