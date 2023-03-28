---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new OutcomesRequestBuilderGetRequestConfiguration();

$queryParameters = new OutcomesRequestBuilderGetQueryParameters();
$queryParameters->filter = "isof('microsoft.graph.educationFeedbackResourceOutcome')";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->outcomes()->get($requestConfiguration);


```