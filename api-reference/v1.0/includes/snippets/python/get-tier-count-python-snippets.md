---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserRequestBuilder.UserRequestBuilderGetQueryParameters(
		count = true,
		orderby = ["displayName"],
		search = "\"displayName:tier\"",
		select = ["displayName","id"],
)

request_configuration = UserRequestBuilder.UserRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
			'ConsistencyLevel' : "eventual",
}

)


result = await client.groups_by_id('group-id').transitiveMembers.graphuser.get(request_configuration = request_configuration)


```