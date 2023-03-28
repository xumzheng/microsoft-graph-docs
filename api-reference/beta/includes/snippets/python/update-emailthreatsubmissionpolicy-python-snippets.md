---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EmailThreatSubmissionPolicy();
$requestBody.setIsReportToMicrosoftEnabled(false);



$requestResult = $graphServiceClient.security().threatSubmission().emailThreatSubmissionPoliciesById('emailThreatSubmissionPolicy-id').patch($requestBody);


```