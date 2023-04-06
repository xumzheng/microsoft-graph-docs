---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonName()
request_body.setNickname('Kesha')


request_config = PersonNameRequestBuilderPatchRequestConfiguration(
request_config = PersonNameRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.profile.names_by_id('personName-id').patch(request_body, headers=)


```