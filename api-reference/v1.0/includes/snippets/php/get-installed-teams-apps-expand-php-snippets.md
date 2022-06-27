---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsAppInstallationRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppInstallationRequestBuilderGetQueryParameters();
$queryParameters->expand = 'teamsAppDefinition';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->installedAppsById('teamsAppInstallation-id')->get($requestConfiguration);


```