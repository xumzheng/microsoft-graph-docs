---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new SchemaExtensionsRequestBuilderGetRequestConfiguration();

$queryParameters = new SchemaExtensionsRequestBuilderGetQueryParameters();
$queryParameters.filter = "id eq 'graphlearn_test'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.schemaExtensions().get($requestConfiguration);


```