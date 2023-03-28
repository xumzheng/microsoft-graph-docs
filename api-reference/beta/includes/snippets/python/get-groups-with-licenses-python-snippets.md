---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupsRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","assignedLicenses"];
$queryParameters.filter = "assignedLicenses/any()";
$queryParameters.expand = ["members($select=id,displayName)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.groups().get($requestConfiguration);


```