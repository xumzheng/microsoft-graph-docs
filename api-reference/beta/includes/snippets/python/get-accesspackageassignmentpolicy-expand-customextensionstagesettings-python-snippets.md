---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration(
request_configuration = AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration(query_params=query_params = AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters()
query_params['expand'] = ["customExtensionStageSettings($expand=customExtension)"]

)
query_params = AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters()
query_params['expand'] = ["customExtensionStageSettings($expand=customExtension)"]

)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies_by_id('accessPackageAssignmentPolicy-id').get(request_configuration)


```