---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsTabRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsTabRequestBuilderGetQueryParameters();
$queryParameters->expand = 'teamsApp';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->chatsById('chat-id')->tabsById('teamsTab-id')->get($requestConfiguration);


```