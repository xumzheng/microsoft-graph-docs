---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new B2xUserFlowsRequestBuilderGetRequestConfiguration();

$queryParameters = new B2xUserFlowsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["identityProviders"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identity()->b2xUserFlows()->get($requestConfiguration);


```