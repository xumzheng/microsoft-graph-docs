---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UsersRequestBuilderGetRequestConfiguration();

query_params = UsersRequestBuilderGetQueryParameters();
query_params.select = ["displayName","id"];
query_params.filter = "identities/any";

request_config.queryParameters = query_params;


result = awaitclient.users().get(request_config);


```