---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = EventRequestBuilderGetRequestConfiguration();

query_params = EventRequestBuilderGetQueryParameters();
query_params.select = ["subject","body","bodyPreview"];

headers = [
'Prefer' => 'outlook.body-content-type="text"',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = await client.me().eventsById('event-id').get(request_config);


```