---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserRequestBuilder.UserRequestBuilderGetQueryParameters(
		select = ["ext55gb1l09_msLearnCourses"],
)

request_configuration = UserRequestBuilder.UserRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.users_by_id('user-id').get(request_configuration = request_configuration)


```