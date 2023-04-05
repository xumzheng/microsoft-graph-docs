---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RiskyUsersRequestBuilderGetRequestConfiguration()

query_params = RiskyUsersRequestBuilderGetQueryParameters()
query_params.filter = "userDisplayName eq 'MyTestUser1'"

request_config.queryParameters = query_params


result = await client.identityProtection.riskyUsers.get(request_config)


```