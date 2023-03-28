---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AppliesToRequestBuilderGetRequestConfiguration();

$queryParameters = new AppliesToRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","appId","displayName","createdDateTime"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.policies().appManagementPoliciesById('appManagementPolicy-id').appliesTo().get($requestConfiguration);


```