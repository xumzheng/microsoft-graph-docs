---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamsAppInstallationRequestBuilderGetRequestConfiguration();

query_params = TeamsAppInstallationRequestBuilderGetQueryParameters();
query_params.expand = ["teamsAppDefinition"];

request_config.queryParameters = query_params;


result = awaitclient.teamsById('team-id').installedAppsById('teamsAppInstallation-id').get(request_config);


```