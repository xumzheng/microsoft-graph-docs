---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonName()
request_body.nickname = 'Kesha'



request_configuration = PersonNameRequestBuilderPatchRequestConfiguration(
)


result = await client.me.profile.names_by_id('personName-id').patch(request_body = request_body)


```