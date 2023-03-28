---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters.filter = "id eq '876df28f-2e78-423b-94a5-44181bd0e225'";
$queryParameters.expand = ["appDefinitions"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.appCatalogs().teamsApps().get($requestConfiguration);


```