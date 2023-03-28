---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UrlThreatSubmission();
$requestBody.set@odatatype('#microsoft.graph.urlThreatSubmission');

$requestBody.setCategory(new SubmissionCategory('phishing'));

$requestBody.setWebUrl('http://phishing.contoso.com');



$requestResult = $graphServiceClient.security().threatSubmission().urlThreats().post($requestBody);


```