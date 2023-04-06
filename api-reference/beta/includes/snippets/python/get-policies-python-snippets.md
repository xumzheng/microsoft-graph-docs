---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PoliciesRequestBuilderGetRequestConfiguration(
request_configuration = PoliciesRequestBuilderGetRequestConfiguration(query_params=query_params = PoliciesRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'"

)
query_params = PoliciesRequestBuilderGetQueryParameters()
query_params['filter'] = "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'"

)


result = await client.identity.conditionalAccess.policies.get(request_configuration)


```