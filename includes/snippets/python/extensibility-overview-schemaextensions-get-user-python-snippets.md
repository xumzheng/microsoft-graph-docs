---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserRequestBuilderGetRequestConfiguration(
query_params = UserRequestBuilderGetQueryParameters()
query_params.select = ["id","displayName","extkmpdyld2_graphLearnCourses"]

)


result = await client.users_by_id('user-id').get(request_config)


```