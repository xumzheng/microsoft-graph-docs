---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration()

query_params = AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters()
query_params.expand = ["customExtensionHandlers($expand=customExtension)"]

request_config.queryParameters = query_params


result = await client.identityGovernance_entitlementManagement_accessPackageAssignmentPoliciesby_id('accessPackageAssignmentPolicy-id').get(request_config)


```