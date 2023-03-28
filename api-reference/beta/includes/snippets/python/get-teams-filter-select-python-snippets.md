---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsRequestBuilderGetQueryParameters();
$queryParameters.filter = "displayName eq 'A Contoso Team'";
$queryParameters.select = ["id","description"];

$requestConfiguration.queryParameters = $queryParameters;


$graphServiceClient.teams().get($requestConfiguration);


```