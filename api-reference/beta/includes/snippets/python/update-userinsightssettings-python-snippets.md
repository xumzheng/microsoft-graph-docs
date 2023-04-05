---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserInsightsSettings()
request_body.setIsEnabled(false)



result = await client.usersby_id('user-id')_settings_itemInsights.patch(request_body)


```