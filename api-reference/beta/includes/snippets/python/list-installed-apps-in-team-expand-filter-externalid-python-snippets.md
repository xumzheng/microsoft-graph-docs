---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new InstalledAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new InstalledAppsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["teamsApp","teamsAppDefinition"];
$queryParameters.filter = "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.teamsById('team-id').installedApps().get($requestConfiguration);


```