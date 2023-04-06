---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration(
request_config = CloudPcOnPremisesConnectionRequestBuilderGetRequestConfiguration(query_params=query_params = CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters()
query_params.select = ["id","displayName","healthCheckStatus","healthCheckStatusDetails","inUse"]

)
query_params = CloudPcOnPremisesConnectionRequestBuilderGetQueryParameters()
query_params.select = ["id","displayName","healthCheckStatus","healthCheckStatusDetails","inUse"]

)


result = await client.deviceManagement.virtualEndpoint.onPremisesConnections_by_id('cloudPcOnPremisesConnection-id').get(request_config, headers=request_config)


```