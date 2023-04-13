---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = CloudPcProvisioningPolicyRequestBuilder.CloudPcProvisioningPolicyRequestBuilderGetQueryParameters(
		expand = ["assignments"],
)

request_configuration = CloudPcProvisioningPolicyRequestBuilder.CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.deviceManagement.virtualEndpoint.provisioningPolicies_by_id('cloudPcProvisioningPolicy-id').get(request_configuration = request_configuration)


```