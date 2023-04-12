---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UrlThreatSubmission()
request_body.@odatatype = '#microsoft.graph.urlThreatSubmission'

request_body.Category(SubmissionCategory('phishing'))

request_body.webUrl = 'http://phishing.contoso.com'




result = await client.security.threatSubmission.urlThreats.post(request_body = request_body)


```