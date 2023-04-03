---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamsAppsRequestBuilderGetRequestConfiguration();

query_params = TeamsAppsRequestBuilderGetQueryParameters();
query_params.filter = "id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'";

request_config.queryParameters = query_params;


result = awaitclient.appCatalogs().teamsApps().get(request_config);


```