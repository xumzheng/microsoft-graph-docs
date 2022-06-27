---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'id%20eq%20\'876df28f-2e78-423b-94a5-44181bd0e225\'';
$queryParameters->expand = 'appDefinitions';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->appCatalogs()->teamsApps()->get($requestConfiguration);


```