---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = InstalledAppsRequestBuilderGetRequestConfiguration();

query_params = InstalledAppsRequestBuilderGetQueryParameters();
query_params.expand = ["teamsAppDefinition"];

request_config.queryParameters = query_params;


result = awaitclient.usersById('user-id').teamwork().installedApps().get(request_config);


```