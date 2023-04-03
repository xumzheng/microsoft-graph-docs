---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = GroupsRequestBuilderGetRequestConfiguration();

query_params = GroupsRequestBuilderGetQueryParameters();
query_params.filter = "graphlearn_courses/courseId eq '123'";
query_params.select = ["displayName","id","description","graphlearn_courses"];

request_config.queryParameters = query_params;


result = await client.groups().get(request_config);


```