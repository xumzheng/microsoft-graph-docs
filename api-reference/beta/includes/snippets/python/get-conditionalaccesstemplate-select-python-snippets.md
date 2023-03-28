---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ConditionalAccessTemplateRequestBuilderGetRequestConfiguration();

$queryParameters = new ConditionalAccessTemplateRequestBuilderGetQueryParameters();
$queryParameters.select = ["details"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identity().conditionalAccess().templatesById('conditionalAccessTemplate-id').get($requestConfiguration);


```