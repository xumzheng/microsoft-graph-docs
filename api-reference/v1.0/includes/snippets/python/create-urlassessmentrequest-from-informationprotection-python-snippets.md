---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ThreatAssessmentRequest();
$requestBody->set@odatatype('#microsoft.graph.urlAssessmentRequest');

$requestBody->setExpectedAssessment(new ThreatExpectedAssessment('block'));

$requestBody->setCategory(new ThreatCategory('phishing'));

$additionalData = [
'url' => 'http://test.com', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->informationProtection()->threatAssessmentRequests()->post($requestBody);


```