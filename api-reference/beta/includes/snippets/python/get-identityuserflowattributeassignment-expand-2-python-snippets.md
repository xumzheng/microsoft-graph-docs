---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UserAttributeAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new UserAttributeAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["userAttribute"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userAttributeAssignments()->get($requestConfiguration);


```