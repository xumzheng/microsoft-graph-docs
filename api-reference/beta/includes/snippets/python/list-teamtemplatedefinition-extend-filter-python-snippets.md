---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamTemplatesRequestBuilderGetRequestConfiguration();

query_params = TeamTemplatesRequestBuilderGetQueryParameters();
query_params.expand = ["definitions"];
query_params.filter = "definitions/any";

request_config.queryParameters = query_params;


result = awaitclient.teamwork().teamTemplates().get(request_config);


```