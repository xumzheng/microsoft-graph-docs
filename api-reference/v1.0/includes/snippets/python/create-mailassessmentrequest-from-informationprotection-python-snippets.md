---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ThreatAssessmentRequest()
request_body.@odatatype = '#microsoft.graph.mailAssessmentRequest'

request_body.ExpectedAssessment(ThreatExpectedAssessment('block'))

request_body.Category(ThreatCategory('spam'))

additionalData = [
'recipientEmail' => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com', 
'messageUri' => 'https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=', 
];
request_body.additionaldata(additionalData)





result = await client.informationProtection.threatAssessmentRequests.post(request_body = request_body)


```