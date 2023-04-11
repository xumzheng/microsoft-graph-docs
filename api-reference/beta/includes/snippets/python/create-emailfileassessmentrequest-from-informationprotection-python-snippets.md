---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ThreatAssessmentRequest()
request_body.@odatatype = '#microsoft.graph.emailFileAssessmentRequest'

request_body.ExpectedAssessment(ThreatExpectedAssessment('block'))

request_body.Category(ThreatCategory('malware'))

additionalData = [
'recipientEmail' => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com', 
'contentData' => 'UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....', 
];
request_body.additionaldata(additionalData)




request_configuration = ThreatAssessmentRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.informationProtection.threatAssessmentRequests.post(request_body = request_body)


```