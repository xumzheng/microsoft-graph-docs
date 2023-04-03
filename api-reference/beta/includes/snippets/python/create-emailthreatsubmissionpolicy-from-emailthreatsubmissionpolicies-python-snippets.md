---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EmailThreatSubmissionPolicy();
requestBody.setIsReportToMicrosoftEnabled(true);



result = await client.security().threatSubmission().emailThreatSubmissionPolicies().post(requestBody);


```