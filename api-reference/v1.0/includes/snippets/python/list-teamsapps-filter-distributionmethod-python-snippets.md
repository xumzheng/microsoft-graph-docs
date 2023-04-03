---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamsAppsRequestBuilderGetRequestConfiguration();

query_params = TeamsAppsRequestBuilderGetQueryParameters();
query_params.filter = "distributionMethod eq 'organization'";

request_config.queryParameters = query_params;


result = awaitclient.appCatalogs().teamsApps().get(request_config);


```