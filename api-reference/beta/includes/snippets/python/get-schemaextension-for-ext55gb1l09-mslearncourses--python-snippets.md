---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserRequestBuilderGetRequestConfiguration(
request_config = UserRequestBuilderGetRequestConfiguration(query_params=query_params = UserRequestBuilderGetQueryParameters()
query_params.select = ["ext55gb1l09_msLearnCourses"]

)
query_params = UserRequestBuilderGetQueryParameters()
query_params.select = ["ext55gb1l09_msLearnCourses"]

)


result = await client.users_by_id('user-id').get(request_config, headers=request_config)


```