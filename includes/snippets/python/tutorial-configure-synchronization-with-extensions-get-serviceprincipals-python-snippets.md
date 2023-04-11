---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ServicePrincipalsRequestBuilder.ServicePrincipalsRequestBuilderGetQueryParameters(
				select = ["id","appId","displayName"],
				filter = "startswith(displayName,%20'salesforce')",
)

request_configuration = ServicePrincipalsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
								'Authorization' : "Bearer {Token}",
}

)


result = await client.servicePrincipals.get(request_configuration = request_configuration)


```