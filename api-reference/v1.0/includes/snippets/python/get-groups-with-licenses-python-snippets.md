---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = GroupsRequestBuilderGetRequestConfiguration(
request_configuration = GroupsRequestBuilderGetRequestConfiguration(query_params=query_params = GroupsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","assignedLicenses"]
query_params['filter'] = "assignedLicenses/any()"
query_params['expand'] = ["members($select=id,displayName)"]

)
query_params = GroupsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","assignedLicenses"]
query_params['filter'] = "assignedLicenses/any()"
query_params['expand'] = ["members($select=id,displayName)"]

)


result = await client.groups.get(request_configuration)


```