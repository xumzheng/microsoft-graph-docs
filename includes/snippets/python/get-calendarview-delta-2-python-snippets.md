---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=params['skiptoken'] = "R0usmcCM996atia_s"
)
headers['Prefer'] = "odata.maxpagesize=2"


result = await client.me.calendarView.delta.get(request_config, headers=request_config)


```