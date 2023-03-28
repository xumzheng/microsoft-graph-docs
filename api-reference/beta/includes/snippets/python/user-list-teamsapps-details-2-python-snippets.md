---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new InstalledAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new InstalledAppsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["teamsAppDefinition($expand=bot)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.usersById('user-id').teamwork().installedApps().get($requestConfiguration);


```