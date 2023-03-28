---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EmailThreatSubmissionPolicy();
$requestBody.setIsReportToMicrosoftEnabled(true);



$requestResult = $graphServiceClient.security().threatSubmission().emailThreatSubmissionPolicies().post($requestBody);


```