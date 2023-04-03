---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EmailThreatSubmissionPolicy();
requestBody.setIsReportToMicrosoftEnabled(false);



result = await client.security().threatSubmission().emailThreatSubmissionPoliciesById('emailThreatSubmissionPolicy-id').patch(requestBody);


```