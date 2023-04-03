---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UrlThreatSubmission();
requestBody.set@odatatype('#microsoft.graph.urlThreatSubmission');

requestBody.setCategory(SubmissionCategory('phishing'));

requestBody.setWebUrl('http://phishing.contoso.com');



result = await client.security().threatSubmission().urlThreats().post(requestBody);


```