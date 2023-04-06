---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceUpdate()
request_body.set@odataid('https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0')


request_config = RefRequestBuilderPutRequestConfiguration(
request_config = RefRequestBuilderPutRequestConfiguration(query_params=)


await client.users_by_id('user-id').manager.ref.put(request_body, headers=)


```