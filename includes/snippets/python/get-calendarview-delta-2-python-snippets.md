---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters.skiptoken = "R0usmcCM996atia_s";

$headers = [
'Prefer' => 'odata.maxpagesize=2',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.me().calendarView().delta().get($requestConfiguration);


```