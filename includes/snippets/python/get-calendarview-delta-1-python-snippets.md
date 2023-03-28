---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters.startdatetime = "2016-12-01T00:00:00Z";
$queryParameters.enddatetime = "2016-12-30T00:00:00Z";

$headers = [
'Prefer' => 'odata.maxpagesize=2',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.me().calendarView().delta().get($requestConfiguration);


```