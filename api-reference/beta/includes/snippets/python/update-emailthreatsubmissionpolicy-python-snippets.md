---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EmailThreatSubmissionPolicy();
requestBody.setIsReportToMicrosoftEnabled(false);



result = awaitclient.security().threatSubmission().emailThreatSubmissionPoliciesById('emailThreatSubmissionPolicy-id').patch(requestBody);


```