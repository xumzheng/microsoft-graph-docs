---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration(
request_configuration = CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration(query_params=query_params = CloudPcProvisioningPolicyRequestBuilderGetQueryParameters()
query_params['select'] = ["id","description","displayName","displayName","domainJoinConfiguration","imageDisplayName","imageId","imageType","onPremisesConnectionId","windowsSettings","managedBy","cloudPcGroupDisplayName","gracePeriodInHours","localAdminEnabled","alternateResourceUrl"]

)
query_params = CloudPcProvisioningPolicyRequestBuilderGetQueryParameters()
query_params['select'] = ["id","description","displayName","displayName","domainJoinConfiguration","imageDisplayName","imageId","imageType","onPremisesConnectionId","windowsSettings","managedBy","cloudPcGroupDisplayName","gracePeriodInHours","localAdminEnabled","alternateResourceUrl"]

)


result = await client.deviceManagement.virtualEndpoint.provisioningPolicies_by_id('cloudPcProvisioningPolicy-id').get(request_configuration)


```