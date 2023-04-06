---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'"
params['count'] = true
params['select'] = ["id","membershipRule","membershipRuleProcessingState"]
)


result = await client.groups.get(request_config, headers=request_config)


```