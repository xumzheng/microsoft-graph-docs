---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ApplicationRequestBuilderGetRequestConfiguration();

$queryParameters = new ApplicationRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","appId","displayName","requiredResourceAccess"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.applicationsById('application-id').get($requestConfiguration);


```