---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ServicePrincipalsRequestBuilderGetRequestConfiguration(
request_configuration = ServicePrincipalsRequestBuilderGetRequestConfiguration(query_params=query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName"]
query_params['filter'] = "startswith(displayName,%20'salesforce')"

)
query_params = ServicePrincipalsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName"]
query_params['filter'] = "startswith(displayName,%20'salesforce')"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.servicePrincipals.get(request_configuration)


```