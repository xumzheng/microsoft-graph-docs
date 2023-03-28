---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters();
$queryParameters->filter = "name eq 'Project' and status eq 'Available'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->directory()->customSecurityAttributeDefinitions()->get($requestConfiguration);


```