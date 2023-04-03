---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UsersRequestBuilderGetRequestConfiguration();

queryParameters = UsersRequestBuilderGetQueryParameters();
queryParameters.count = true;
queryParameters.select = ["id","displayName","customSecurityAttributes"];
queryParameters.filter = "startsWith(customSecurityAttributes/Marketing/EmployeeId,'GS')";

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.users().get(requestConfiguration);


```