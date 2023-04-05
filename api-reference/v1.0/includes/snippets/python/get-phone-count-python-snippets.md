---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ContactsRequestBuilderGetRequestConfiguration(
query_params = ContactsRequestBuilderGetQueryParameters()
query_params.search = "\"displayName:wa\""
query_params.count = true

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.contacts.get(request_config)


```