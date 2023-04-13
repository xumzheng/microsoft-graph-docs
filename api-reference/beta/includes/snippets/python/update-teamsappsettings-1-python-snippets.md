---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsAppSettings()
request_body.@odatatype = '#microsoft.graph.teamsAppSettings'

request_body.is_chat_resource_specific_consent_enabled = True




result = await client.teamwork.teamsAppSettings.patch(request_body = request_body)


```