---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["appDefinitions($select=id,displayName,allowedInstallationScopes)"];
$queryParameters.filter = "appDefinitions/any";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.appCatalogs().teamsApps().get($requestConfiguration);


```