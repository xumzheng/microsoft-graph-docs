---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration();

query_params = CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters();
query_params.select = ["id","displayName","healthCheckStatus","healthCheckStatusDetails","inUse"];

request_config.queryParameters = query_params;


result = awaitclient.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').get(request_config);


```