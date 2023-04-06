---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UsersRequestBuilderGetRequestConfiguration(
request_configuration = UsersRequestBuilderGetRequestConfiguration(query_params=query_params = UsersRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['consistencyLevel'] = "eventual"
query_params['filter'] = "endsWith(mail,'@contoso.com')"

)
query_params = UsersRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['consistencyLevel'] = "eventual"
query_params['filter'] = "endsWith(mail,'@contoso.com')"

)


result = await client.users.get(request_configuration)


```