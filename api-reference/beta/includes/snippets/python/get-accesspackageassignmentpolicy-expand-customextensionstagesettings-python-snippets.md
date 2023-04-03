---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration();

query_params = AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters();
query_params.expand = ["customExtensionStageSettings($expand=customExtension)"];

request_config.queryParameters = query_params;


result = awaitclient.identityGovernance().entitlementManagement().accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id').get(request_config);


```