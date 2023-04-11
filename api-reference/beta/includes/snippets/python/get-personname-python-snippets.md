---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PersonNameRequestBuilderGetRequestConfiguration(
)


result = await client.me.profile.names_by_id('personName-id').get()


```