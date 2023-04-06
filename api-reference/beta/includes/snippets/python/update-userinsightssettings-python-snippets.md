---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserInsightsSettings()
request_body.setIsEnabled(false)


request_config = ItemInsightsRequestBuilderPatchRequestConfiguration(
request_config = ItemInsightsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.users_by_id('user-id').settings.itemInsights.patch(request_body, headers=)


```