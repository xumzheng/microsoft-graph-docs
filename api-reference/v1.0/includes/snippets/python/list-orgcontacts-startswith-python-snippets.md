---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ContactsRequestBuilderGetRequestConfiguration();

$queryParameters = new ContactsRequestBuilderGetQueryParameters();
$queryParameters.filter = "startswith(displayName,'A')";
$queryParameters.count = true;
$queryParameters.top = 1;
$queryParameters.orderby = ["displayName"];

$headers = [
'ConsistencyLevel' => 'eventual',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.contacts().get($requestConfiguration);


```