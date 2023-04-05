---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EmailThreatSubmissionPolicy()
request_body.setIsReportToMicrosoftEnabled(true)



result = await client.security.threatSubmission.emailThreatSubmissionPolicies.post(request_body)


```