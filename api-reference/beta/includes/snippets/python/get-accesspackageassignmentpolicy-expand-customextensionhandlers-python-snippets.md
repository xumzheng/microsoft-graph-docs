---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration();

queryParameters = AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters();
queryParameters.expand = ["customExtensionHandlers($expand=customExtension)"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id').get(requestConfiguration);


```