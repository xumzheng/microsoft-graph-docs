---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WebAccount()
request_body.setWebUrl('https://github.com/innocenty.popov')


request_config = WebAccountRequestBuilderPatchRequestConfiguration(
request_config = WebAccountRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.profile.webAccounts_by_id('webAccount-id').patch(request_body, headers=)


```