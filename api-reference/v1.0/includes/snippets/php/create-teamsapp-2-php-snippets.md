---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsAppsRequestBuilderPostRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderPostQueryParameters();
$queryParameters->requiresReview = true;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->appCatalogs()->teamsApps()->post($requestConfiguration);


```