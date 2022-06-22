---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new InstalledAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new InstalledAppsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'teamsApp,teamsAppDefinition';
$queryParameters->filter = 'teamsApp/externalId%20eq%20\'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->installedApps()->get($requestConfiguration);


```