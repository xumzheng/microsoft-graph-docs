---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = InstalledAppsRequestBuilderGetRequestConfiguration();

query_params = InstalledAppsRequestBuilderGetQueryParameters();
query_params.expand = ["teamsAppDefinition($expand=bot)"];

request_config.queryParameters = query_params;


result = awaitclient.chatsById('chat-id').installedApps().get(request_config);


```