---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = InstalledAppsRequestBuilderGetRequestConfiguration();

query_params = InstalledAppsRequestBuilderGetQueryParameters;
query_params.expand = ["teamsApp","teamsAppDefinition"];
query_params.filter = "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'";

request_config.queryParameters = query_params;


result = await client.usersById('user-id').teamwork().installedApps().get(request_config);


```