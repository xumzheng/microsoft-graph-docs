---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration();

queryParameters = IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters();
queryParameters.expand = ["userAttribute"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id').get(requestConfiguration);


```