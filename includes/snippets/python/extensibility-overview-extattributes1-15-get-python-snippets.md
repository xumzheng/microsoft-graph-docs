---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UsersRequestBuilderGetRequestConfiguration();

queryParameters = UsersRequestBuilderGetQueryParameters();
queryParameters.select = ["id","displayName","onPremisesExtensionAttributes"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.users().get(requestConfiguration);


```