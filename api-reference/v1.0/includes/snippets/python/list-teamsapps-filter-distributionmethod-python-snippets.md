---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsAppsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsAppsRequestBuilderGetQueryParameters();
$queryParameters.filter = "distributionMethod eq 'organization'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.appCatalogs().teamsApps().get($requestConfiguration);


```