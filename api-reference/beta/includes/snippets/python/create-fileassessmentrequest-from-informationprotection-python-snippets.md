---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ThreatAssessmentRequest()
request_body.@odatatype = '#microsoft.graph.fileAssessmentRequest'

request_body.ExpectedAssessment(ThreatExpectedAssessment('block'))

request_body.Category(ThreatCategory('malware'))

additionalData = [
'fileName' => 'test.txt', 
'contentData' => 'VGhpcyBpcyBhIHRlc3QgZmlsZQ==', 
];
request_body.additionaldata(additionalData)





result = await client.informationProtection.threatAssessmentRequests.post(request_body = request_body)


```