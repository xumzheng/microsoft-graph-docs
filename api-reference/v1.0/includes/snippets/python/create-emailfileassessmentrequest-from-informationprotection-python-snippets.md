---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ThreatAssessmentRequest();
requestBody.set@odatatype('#microsoft.graph.emailFileAssessmentRequest');

requestBody.setExpectedAssessment(ThreatExpectedAssessment('block'));

requestBody.setCategory(ThreatCategory('malware'));

additionalData = [
'recipientEmail' => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com', 
'contentData' => 'UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.informationProtection().threatAssessmentRequests().post(requestBody);


```