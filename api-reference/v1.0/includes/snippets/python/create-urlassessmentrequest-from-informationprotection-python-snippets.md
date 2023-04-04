---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ThreatAssessmentRequest()
request_body.set@odatatype('#microsoft.graph.urlAssessmentRequest')

request_body.setExpectedAssessment(ThreatExpectedAssessment('block'))

request_body.setCategory(ThreatCategory('phishing'))

additionalData = [
'url' => 'http://test.com', 
];
request_body.setAdditionalData(additionalData)




result = await client.informationProtection.threatAssessmentRequests.post(request_body)


```