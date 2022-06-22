---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new InstalledAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new InstalledAppsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'teamsAppDefinition($expand=bot)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->chatsById('chat-id')->installedApps()->get($requestConfiguration);


```