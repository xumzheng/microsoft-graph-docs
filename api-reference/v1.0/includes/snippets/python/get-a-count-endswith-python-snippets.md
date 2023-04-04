---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UsersRequestBuilderGetRequestConfiguration()

query_params = UsersRequestBuilderGetQueryParameters()
query_params.filter = "endswith(mail,'a@contoso.com')"
query_params.orderby = ["userPrincipalName"]
query_params.count = true

headers = [
'ConsistencyLevel' => 'eventual',
]

request_config.queryParameters = query_params
request_config.headers = headers


result = await client.users.get(request_config)


```