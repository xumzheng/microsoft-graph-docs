---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = GroupsRequestBuilderGetRequestConfiguration();

query_params = GroupsRequestBuilderGetQueryParameters();
query_params.select = ["id","assignedLicenses"];
query_params.filter = "assignedLicenses/any()";
query_params.expand = ["members($select=id,displayName)"];

request_config.queryParameters = query_params;


result = awaitclient.groups().get(request_config);


```