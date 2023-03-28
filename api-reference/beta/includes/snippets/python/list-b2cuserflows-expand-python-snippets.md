---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new B2cUserFlowsRequestBuilderGetRequestConfiguration();

$queryParameters = new B2cUserFlowsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["identityProviders"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identity().b2cUserFlows().get($requestConfiguration);


```