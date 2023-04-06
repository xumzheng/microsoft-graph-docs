---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["displayName"]
)
headers['Prefer'] = "odata.maxpagesize=2"


result = await client.me.contactFolders_by_id('contactFolder-id').contacts.delta.get(request_config, headers=request_config)


```