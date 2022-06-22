---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration();

$queryParameters = new UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters();
$queryParameters->expand = 'teamsAppDefinition';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->usersById('user-id')->teamwork()->installedAppsById('userScopeTeamsAppInstallation-id')->get($requestConfiguration);


```