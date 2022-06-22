---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MembersRequestBuilderGetRequestConfiguration();

$queryParameters = new MembersRequestBuilderGetQueryParameters();
$queryParameters->filter = '(microsoft.graph.aadUserConversationMember/userId%20eq%20\'73761f06-2ac9-469c-9f10-279a8cc267f9\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->members()->get($requestConfiguration);


```