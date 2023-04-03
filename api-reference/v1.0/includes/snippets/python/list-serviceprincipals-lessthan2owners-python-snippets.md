---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServicePrincipalsRequestBuilderGetRequestConfiguration();

queryParameters = ServicePrincipalsRequestBuilderGetQueryParameters();
queryParameters.filter = "owners/$count eq 0 or owners/$count eq 1";
queryParameters.count = true;
queryParameters.select = ["id","displayName"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.servicePrincipals().get(requestConfiguration);


```