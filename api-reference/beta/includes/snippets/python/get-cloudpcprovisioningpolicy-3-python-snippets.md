---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration()

query_params = CloudPcProvisioningPolicyRequestBuilderGetQueryParameters()
query_params.select = ["id","description","displayName","displayName","domainJoinConfiguration","imageDisplayName","imageId","imageType","onPremisesConnectionId","windowsSettings","managedBy","cloudPcGroupDisplayName","gracePeriodInHours","localAdminEnabled","alternateResourceUrl"]

request_config.queryParameters = query_params


result = await client.deviceManagement_virtualEndpoint_provisioningPoliciesby_id('cloudPcProvisioningPolicy-id').get(request_config)


```