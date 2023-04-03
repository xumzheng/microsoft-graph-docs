---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PeopleRequestBuilderGetRequestConfiguration();

query_params = PeopleRequestBuilderGetQueryParameters();
query_params.search = "\"Irene McGowen\"";

request_config.queryParameters = query_params;


result = awaitclient.me().people().get(request_config);


```