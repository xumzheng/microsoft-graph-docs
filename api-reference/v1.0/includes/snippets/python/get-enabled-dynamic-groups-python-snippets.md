---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = GroupsRequestBuilderGetRequestConfiguration()

query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'"
query_params.count = true
query_params.select = ["id","membershipRule","membershipRuleProcessingState"]

headers = [
'ConsistencyLevel' => 'eventual',
]

request_config.queryParameters = query_params
request_config.headers = headers


result = await client.groups.get(request_config)


```