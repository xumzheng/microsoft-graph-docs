---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UnifiedRoleManagementPolicyRequestBuilderGetRequestConfiguration();

queryParameters = UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters();
queryParameters.expand = ["effectiveRules","rules"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.policies().roleManagementPoliciesById('unifiedRoleManagementPolicy-id').get(requestConfiguration);


```