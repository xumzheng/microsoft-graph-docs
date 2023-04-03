---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamsRequestBuilderGetRequestConfiguration();

query_params = TeamsRequestBuilderGetQueryParameters();
query_params.filter = "displayName eq 'A Contoso Team'";
query_params.select = ["id","description"];

request_config.queryParameters = query_params;


awaitclient.teams().get(request_config);


```