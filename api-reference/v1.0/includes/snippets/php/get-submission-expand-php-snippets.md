---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new EducationSubmissionRequestBuilderGetRequestConfiguration();

$queryParameters = new EducationSubmissionRequestBuilderGetQueryParameters();
$queryParameters->expand = '*';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->get($requestConfiguration);


```