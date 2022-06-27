---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'id%20eq%20\'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->appCatalogs()->teamsApps()->get($requestConfiguration);


```