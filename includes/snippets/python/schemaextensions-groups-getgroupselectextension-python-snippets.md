---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupsRequestBuilderGetRequestConfiguration();

queryParameters = GroupsRequestBuilderGetQueryParameters();
queryParameters.filter = "graphlearn_courses/courseId eq '123'";
queryParameters.select = ["displayName","id","description","graphlearn_courses"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.groups().get(requestConfiguration);


```