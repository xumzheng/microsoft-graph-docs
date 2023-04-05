---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration(
query_params = CloudPcProvisioningPolicyRequestBuilderGetQueryParameters()
query_params.expand = ["assignments"]

)


result = await client.deviceManagement.virtualEndpoint.provisioningPolicies_by_id('cloudPcProvisioningPolicy-id').get(request_config)


```