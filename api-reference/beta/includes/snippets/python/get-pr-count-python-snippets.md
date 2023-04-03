---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UserRequestBuilderGetRequestConfiguration();

queryParameters = UserRequestBuilderGetQueryParameters();
queryParameters.count = true;
queryParameters.orderby = ["displayName"];
queryParameters.search = "\"displayName:Pr\"";
queryParameters.select = ["displayName","id"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groupsById('group-id').members().graphUser().get(requestConfiguration);


```