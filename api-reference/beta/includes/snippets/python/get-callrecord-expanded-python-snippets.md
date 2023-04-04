---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = CallRecordRequestBuilderGetRequestConfiguration();

query_params = CallRecordRequestBuilderGetQueryParameters();
query_params.expand = ["sessions($expand=segments)"];

request_config.queryParameters = query_params;


result = await client.communications.callRecordsById('callRecord-id').get(request_config);


```