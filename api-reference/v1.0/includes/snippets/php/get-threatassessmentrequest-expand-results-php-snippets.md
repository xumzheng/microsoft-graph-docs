---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ThreatAssessmentRequestRequestBuilderGetRequestConfiguration();

$queryParameters = new ThreatAssessmentRequestRequestBuilderGetQueryParameters();
$queryParameters->expand = 'results';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->informationProtection()->threatAssessmentRequestsById('threatAssessmentRequest-id')->get($requestConfiguration);


```