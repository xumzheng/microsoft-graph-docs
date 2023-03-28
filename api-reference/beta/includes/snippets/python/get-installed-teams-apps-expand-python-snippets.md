---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsAppInstallationRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppInstallationRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsAppDefinition"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->teamsById('team-id')->installedAppsById('teamsAppInstallation-id')->get($requestConfiguration);


```