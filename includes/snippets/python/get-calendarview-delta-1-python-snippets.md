---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=query_params = DeltaRequestBuilderGetQueryParameters()
query_params.startdatetime = "2016-12-01T00:00:00Z"
query_params.enddatetime = "2016-12-30T00:00:00Z"

)
query_params = DeltaRequestBuilderGetQueryParameters()
query_params.startdatetime = "2016-12-01T00:00:00Z"
query_params.enddatetime = "2016-12-30T00:00:00Z"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.calendarView.delta.get(request_config, headers=request_config)


```