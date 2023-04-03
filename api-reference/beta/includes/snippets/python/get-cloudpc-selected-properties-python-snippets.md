---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = CloudPCRequestBuilderGetRequestConfiguration();

queryParameters = CloudPCRequestBuilderGetQueryParameters();
queryParameters.select = ["id","displayName","imageDisplayName","lastModifiedDateTime","lastRemoteActionResult","lastLoginResult","connectivityResult"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').get(requestConfiguration);


```