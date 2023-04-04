---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AppliesToRequestBuilderGetRequestConfiguration();

query_params = AppliesToRequestBuilderGetQueryParameters();
query_params.select = ["id","appId","displayName","createdDateTime"];

request_config.queryParameters = query_params;


result = await client.policies.appManagementPoliciesById('appManagementPolicy-id').appliesTo.get(request_config);


```