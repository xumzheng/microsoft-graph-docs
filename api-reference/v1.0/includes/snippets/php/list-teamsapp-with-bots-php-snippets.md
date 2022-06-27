---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'appDefinitions($expand=bot)';
$queryParameters->filter = 'appDefinitions/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->appCatalogs()->teamsApps()->get($requestConfiguration);


```