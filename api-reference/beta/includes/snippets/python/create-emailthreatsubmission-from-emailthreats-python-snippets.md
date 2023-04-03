---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EmailThreatSubmission();
requestBody.set@odatatype('#microsoft.graph.emailUrlThreatSubmission');

requestBody.setCategory(SubmissionCategory('spam'));

requestBody.setRecipientEmailAddress('tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com');

additionalData = [
'messageUrl' => 'https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.security().threatSubmission().emailThreats().post(requestBody);


```