---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters();
$queryParameters.expand = ["instance($expand=definition)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().accessReviews().decisionsById('accessReviewInstanceDecisionItem-id').get($requestConfiguration);


```