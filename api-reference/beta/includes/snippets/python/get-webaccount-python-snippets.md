---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = WebAccountRequestBuilderGetRequestConfiguration(
)


result = await client.me.profile.webAccounts_by_id('webAccount-id').get()


```