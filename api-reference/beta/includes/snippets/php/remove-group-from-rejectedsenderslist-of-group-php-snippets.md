---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RefRequestBuilderDeleteRequestConfiguration();

$queryParameters = new RefRequestBuilderDeleteQueryParameters();
$queryParameters->id = 'https://graph.microsoft.com/beta/groups/%7Bother-group-id%7D';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->groupsById('group-id')->rejectedSenders()->ref()->delete($requestConfiguration);


```