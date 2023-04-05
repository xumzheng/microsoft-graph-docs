---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Identity()
request_body.setId('e5477431-1038-484e-bf69-1dfedb97a110')

request_body.setType(IdentityType('group'))



result = await client.external.connectionsby_id('externalConnection-id').groupsby_id('externalGroup-id').members.post(request_body)


```