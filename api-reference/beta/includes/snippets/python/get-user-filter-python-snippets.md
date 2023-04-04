---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UsersRequestBuilderGetRequestConfiguration();

query_params = UsersRequestBuilderGetQueryParameters();
query_params.count = true;
query_params.consistencyLevel = "eventual";
query_params.filter = "endsWith(mail,'@contoso.com')";

request_config.queryParameters = query_params;


result = await client.users.get(request_config);


```