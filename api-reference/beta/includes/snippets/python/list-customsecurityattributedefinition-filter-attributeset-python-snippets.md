---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters();
$queryParameters.filter = "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.directory().customSecurityAttributeDefinitions().get($requestConfiguration);


```