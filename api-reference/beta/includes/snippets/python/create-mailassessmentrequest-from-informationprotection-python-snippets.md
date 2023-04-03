---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ThreatAssessmentRequest();
requestBody.set@odatatype('#microsoft.graph.mailAssessmentRequest');

requestBody.setExpectedAssessment(ThreatExpectedAssessment('block'));

requestBody.setCategory(ThreatCategory('spam'));

additionalData = [
'recipientEmail' => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com', 
'messageUri' => 'https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=', 
];
requestBody.setAdditionalData(additionalData);




result = await client.informationProtection().threatAssessmentRequests().post(requestBody);


```