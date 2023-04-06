---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ApplicationsRequestBuilderGetRequestConfiguration(
request_config = ApplicationsRequestBuilderGetRequestConfiguration(query_params=params['search'] = "\"displayName:Web\""
params['count'] = true
params['select'] = ["appId","identifierUris","displayName","publisherDomain","signInAudience"]
)
headers['ConsistencyLevel'] = "eventual"


result = await client.applications.get(request_config, headers=request_config)


```