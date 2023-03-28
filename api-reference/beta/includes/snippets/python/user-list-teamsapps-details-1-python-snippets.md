---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration();

$queryParameters = new UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsAppDefinition"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->usersById('user-id')->teamwork()->installedAppsById('userScopeTeamsAppInstallation-id')->get($requestConfiguration);


```