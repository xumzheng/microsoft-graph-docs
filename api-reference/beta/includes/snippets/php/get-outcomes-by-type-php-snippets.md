---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OutcomesRequestBuilderGetRequestConfiguration();

$queryParameters = new OutcomesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'isof(\'microsoft.graph.educationFeedbackResourceOutcome\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->outcomes()->get($requestConfiguration);


```