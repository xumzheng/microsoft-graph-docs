---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(
)


result = await client.chats_by_id('chat-id').installedApps_by_id('teamsAppInstallation-id').get()


```