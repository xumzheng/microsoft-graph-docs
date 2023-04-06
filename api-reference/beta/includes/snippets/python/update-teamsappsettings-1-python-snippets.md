---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsAppSettings()
request_body.set@odatatype('#microsoft.graph.teamsAppSettings')

request_body.setIsChatResourceSpecificConsentEnabled(true)


request_config = TeamsAppSettingsRequestBuilderPatchRequestConfiguration(
request_config = TeamsAppSettingsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teamwork.teamsAppSettings.patch(request_body, headers=)


```