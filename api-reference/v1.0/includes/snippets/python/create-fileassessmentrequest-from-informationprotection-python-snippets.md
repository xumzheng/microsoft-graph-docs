---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ThreatAssessmentRequest();
requestBody.set@odatatype('#microsoft.graph.fileAssessmentRequest');

requestBody.setExpectedAssessment(ThreatExpectedAssessment('block'));

requestBody.setCategory(ThreatCategory('malware'));

additionalData = [
'fileName' => 'test.txt', 
'contentData' => 'VGhpcyBpcyBhIHRlc3QgZmlsZQ==', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.informationProtection().threatAssessmentRequests().post(requestBody);


```