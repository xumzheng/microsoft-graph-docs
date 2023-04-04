---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UserRequestBuilderGetRequestConfiguration()

query_params = UserRequestBuilderGetQueryParameters()
query_params.select = ["id","displayName","extkmpdyld2_graphLearnCourses"]

request_config.queryParameters = query_params


result = await client.usersById('user-id').get(request_config)


```