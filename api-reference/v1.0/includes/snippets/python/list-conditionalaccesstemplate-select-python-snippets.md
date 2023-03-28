---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TemplatesRequestBuilderGetRequestConfiguration();

$queryParameters = new TemplatesRequestBuilderGetQueryParameters();
$queryParameters->select = ["name","description","id","scenarios"];
$queryParameters->filter = "scenarios has 'secureFoundation'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identity()->conditionalAccess()->templates()->get($requestConfiguration);


```