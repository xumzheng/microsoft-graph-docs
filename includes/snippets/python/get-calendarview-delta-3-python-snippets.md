---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.skiptoken = "R0usmci39OQxqJrxK4";

headers = [
'Prefer' => 'odata.maxpagesize=2',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().calendarView().delta().get(requestConfiguration);


```