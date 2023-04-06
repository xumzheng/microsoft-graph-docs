---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","assignedLicenses"]
params['filter'] = "assignedLicenses/any()"
params['expand'] = ["members($select=id,displayName)"]
)


result = await client.groups.get(request_config, headers=request_config)


```