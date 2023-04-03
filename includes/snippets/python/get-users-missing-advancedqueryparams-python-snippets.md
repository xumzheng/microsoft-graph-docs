---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UsersRequestBuilderGetRequestConfiguration();

queryParameters = UsersRequestBuilderGetQueryParameters();
queryParameters.filter = "endsWith(mail,'@outlook.com')";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.users().get(requestConfiguration);


```