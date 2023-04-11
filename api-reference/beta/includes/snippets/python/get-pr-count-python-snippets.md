---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserRequestBuilder.UserRequestBuilderGetQueryParameters(
		count = true,
		orderby = ["displayName"],
		search = "\"displayName:Pr\"",
		select = ["displayName","id"],
)

request_configuration = UserRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)
headers = {
				'ConsistencyLevel' : "eventual",
}

)


result = await client.groups_by_id('group-id').members.graphuser.get(request_configuration = request_configuration)


```