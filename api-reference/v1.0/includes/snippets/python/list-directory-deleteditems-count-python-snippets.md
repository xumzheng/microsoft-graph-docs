---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters.count = true;
$queryParameters.orderby = ["deletedDateTime asc"];
$queryParameters.select = ["id","DisplayName","deletedDateTime"];

$headers = [
'ConsistencyLevel' => 'eventual',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.directory().deletedItems().graphGroup().get($requestConfiguration);


```