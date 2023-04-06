---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UrlThreatSubmission()
request_body.set@odatatype('#microsoft.graph.urlThreatSubmission')

request_body.setCategory(SubmissionCategory('phishing'))

request_body.setWebUrl('http://phishing.contoso.com')


request_config = UrlThreatsRequestBuilderPostRequestConfiguration(
request_config = UrlThreatsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.threatSubmission.urlThreats.post(request_body, headers=)


```