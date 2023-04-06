---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ContactsRequestBuilderGetRequestConfiguration(
request_config = ContactsRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["displayName","emailAddresses"]
)


result = await client.me.contacts.get(request_config, headers=request_config)


```