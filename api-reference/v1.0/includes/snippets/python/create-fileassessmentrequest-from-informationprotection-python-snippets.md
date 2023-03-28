---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ThreatAssessmentRequest();
$requestBody->set@odatatype('#microsoft.graph.fileAssessmentRequest');

$requestBody->setExpectedAssessment(new ThreatExpectedAssessment('block'));

$requestBody->setCategory(new ThreatCategory('malware'));

$additionalData = [
'fileName' => 'test.txt', 
'contentData' => 'VGhpcyBpcyBhIHRlc3QgZmlsZQ==', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->informationProtection()->threatAssessmentRequests()->post($requestBody);


```