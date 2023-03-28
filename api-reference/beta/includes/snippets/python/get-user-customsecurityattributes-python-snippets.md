---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UserRequestBuilderGetRequestConfiguration();

$queryParameters = new UserRequestBuilderGetQueryParameters();
$queryParameters.select = ["customSecurityAttributes"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.usersById('user-id').get($requestConfiguration);


```