---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/users/alexd@contoso.com')



await client.groups._by_id('group-id').rejectedSenders.ref.post(request_body)


```