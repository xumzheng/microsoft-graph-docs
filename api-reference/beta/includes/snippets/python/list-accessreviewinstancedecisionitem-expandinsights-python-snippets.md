---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DecisionsRequestBuilderGetRequestConfiguration();

$queryParameters = new DecisionsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["insights"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->accessReviews()->definitionsById('accessReviewScheduleDefinition-id')->instancesById('accessReviewInstance-id')->decisions()->get($requestConfiguration);


```