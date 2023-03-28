---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ApplicationTemplatesRequestBuilderGetRequestConfiguration();

$queryParameters = new ApplicationTemplatesRequestBuilderGetQueryParameters();
$queryParameters->filter = "displayName eq 'AWS IAM Identity Center '";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->applicationTemplates()->get($requestConfiguration);


```