---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CloudPcProvisioningPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPcProvisioningPolicyRequestBuilderGetQueryParameters();
$queryParameters.expand = ["assignments"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.deviceManagement().virtualEndpoint().provisioningPoliciesById('cloudPcProvisioningPolicy-id').get($requestConfiguration);


```