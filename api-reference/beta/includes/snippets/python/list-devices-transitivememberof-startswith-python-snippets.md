---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = GroupRequestBuilder.GroupRequestBuilderGetQueryParameters(
		count = true,
		orderby = ["displayName"],
		filter = "startswith(displayName,%20'a')",
)

request_configuration = GroupRequestBuilder.GroupRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)
headers = {
'ConsistencyLevel' : "eventual",
}

)


result = await client.devices_by_id('device-id').transitiveMemberOf.graphgroup.get(request_configuration = request_configuration)


```