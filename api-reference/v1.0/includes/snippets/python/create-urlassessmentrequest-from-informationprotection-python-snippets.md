---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ThreatAssessmentRequest();
requestBody.set@odatatype('#microsoft.graph.urlAssessmentRequest');

requestBody.setExpectedAssessment(ThreatExpectedAssessment('block'));

requestBody.setCategory(ThreatCategory('phishing'));

additionalData = [
'url' => 'http://test.com', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.informationProtection().threatAssessmentRequests().post(requestBody);


```