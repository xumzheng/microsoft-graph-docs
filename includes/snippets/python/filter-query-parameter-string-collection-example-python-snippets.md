---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UsersRequestBuilderGetRequestConfiguration();

$queryParameters = new UsersRequestBuilderGetQueryParameters();
$queryParameters.filter = "imAddresses/any";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.users().get($requestConfiguration);


```