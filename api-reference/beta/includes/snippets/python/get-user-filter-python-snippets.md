---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UsersRequestBuilderGetRequestConfiguration(
request_config = UsersRequestBuilderGetRequestConfiguration(query_params=params['count'] = true
params['consistencyLevel'] = "eventual"
params['filter'] = "endsWith(mail,'@contoso.com')"
)


result = await client.users.get(request_config, headers=request_config)


```