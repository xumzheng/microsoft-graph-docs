---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/v1.0/users/{userId}'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.print.shares_by_id('printerShare-id').allowedUsers.ref.post(request_body = request_body)


```