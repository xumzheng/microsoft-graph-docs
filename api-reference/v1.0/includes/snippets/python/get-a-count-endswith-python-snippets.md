---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UsersRequestBuilderGetRequestConfiguration(
request_configuration = UsersRequestBuilderGetRequestConfiguration(query_params=query_params = UsersRequestBuilderGetQueryParameters()
query_params['filter'] = "endswith(mail,'a@contoso.com')"
query_params['orderby'] = ["userPrincipalName"]
query_params['count'] = true

)
query_params = UsersRequestBuilderGetQueryParameters()
query_params['filter'] = "endswith(mail,'a@contoso.com')"
query_params['orderby'] = ["userPrincipalName"]
query_params['count'] = true

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.users.get(request_configuration)


```