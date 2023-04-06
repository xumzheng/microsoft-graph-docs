---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'"
query_params.count = true
query_params.select = ["id","membershipRule","membershipRuleProcessingState"]

)
query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'"
query_params.count = true
query_params.select = ["id","membershipRule","membershipRuleProcessingState"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups.get(request_config, headers=request_config)


```