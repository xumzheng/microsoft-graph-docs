---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServicePrincipalsRequestBuilderGetRequestConfiguration();

queryParameters = ServicePrincipalsRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:Team\"";
queryParameters.count = true;
queryParameters.select = ["accountEnabled","displayName","publisherName","servicePrincipalType","signInAudience"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.servicePrincipals().get(requestConfiguration);


```