---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CallRecordRequestBuilderGetRequestConfiguration(
request_config = CallRecordRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["sessions($expand=segments)"]
)


result = await client.communications.callRecords_by_id('callRecord-id').get(request_config, headers=request_config)


```