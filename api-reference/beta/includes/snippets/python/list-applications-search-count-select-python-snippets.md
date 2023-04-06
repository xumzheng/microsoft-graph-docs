---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ApplicationsRequestBuilderGetRequestConfiguration(
request_configuration = ApplicationsRequestBuilderGetRequestConfiguration(query_params=query_params = ApplicationsRequestBuilderGetQueryParameters()
query_params['search'] = "\"displayName:Web\""
query_params['count'] = true
query_params['select'] = ["appId","identifierUris","displayName","publisherDomain","signInAudience"]

)
query_params = ApplicationsRequestBuilderGetQueryParameters()
query_params['search'] = "\"displayName:Web\""
query_params['count'] = true
query_params['select'] = ["appId","identifierUris","displayName","publisherDomain","signInAudience"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.applications.get(request_configuration)


```