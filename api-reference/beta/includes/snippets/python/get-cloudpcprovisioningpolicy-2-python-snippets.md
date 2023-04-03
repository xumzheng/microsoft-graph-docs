---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration();

query_params = CloudPcProvisioningPolicyRequestBuilderGetQueryParameters();
query_params.expand = ["assignments"];

request_config.queryParameters = query_params;


result = awaitclient.deviceManagement().virtualEndpoint().provisioningPoliciesById('cloudPcProvisioningPolicy-id').get(request_config);


```