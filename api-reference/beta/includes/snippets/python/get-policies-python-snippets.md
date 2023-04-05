---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PoliciesRequestBuilderGetRequestConfiguration()

query_params = PoliciesRequestBuilderGetQueryParameters()
query_params.filter = "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'"

request_config.queryParameters = query_params


result = await client.identity_conditionalAccess_policies.get(request_config)


```