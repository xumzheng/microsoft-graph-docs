---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new LanguagesRequestBuilderGetRequestConfiguration();

$queryParameters = new LanguagesRequestBuilderGetQueryParameters();
$queryParameters->filter = "isEnabled eq true";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->languages()->get($requestConfiguration);


```