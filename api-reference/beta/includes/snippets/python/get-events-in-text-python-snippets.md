---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = EventsRequestBuilderGetRequestConfiguration();

queryParameters = EventsRequestBuilderGetQueryParameters();
queryParameters.select = ["subject","body","bodyPreview"];

headers = [
'Prefer' => 'outlook.body-content-type="text"',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().events().get(requestConfiguration);


```