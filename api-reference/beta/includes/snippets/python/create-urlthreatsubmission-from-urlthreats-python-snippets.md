---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UrlThreatSubmission();
requestBody.set@odatatype('#microsoft.graph.urlThreatSubmission');

requestBody.setCategory(SubmissionCategory('phishing'));

requestBody.setWebUrl('http://phishing.contoso.com');



result = awaitclient.security().threatSubmission().urlThreats().post(requestBody);


```