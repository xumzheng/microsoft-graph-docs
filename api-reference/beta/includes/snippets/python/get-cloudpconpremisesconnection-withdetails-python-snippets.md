---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration();

queryParameters = CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters();
queryParameters.select = ["id","displayName","healthCheckStatus","healthCheckStatusDetails","inUse"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').get(requestConfiguration);


```