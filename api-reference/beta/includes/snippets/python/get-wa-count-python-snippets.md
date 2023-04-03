---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UsersRequestBuilderGetRequestConfiguration();

queryParameters = UsersRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:wa\"";
queryParameters.orderby = ["displayName"];
queryParameters.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.users().get(requestConfiguration);


```