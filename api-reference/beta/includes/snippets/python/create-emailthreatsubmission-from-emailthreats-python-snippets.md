---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EmailThreatSubmission()
request_body.@odatatype = '#microsoft.graph.emailUrlThreatSubmission'

request_body.Category(SubmissionCategory('spam'))

request_body.recipientEmailAddress = 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com'

additionalData = [
'messageUrl' => 'https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=', 
];
request_body.additionaldata(additionalData)




request_configuration = EmailThreatsRequestBuilderPostRequestConfiguration(
)


result = await client.security.threatSubmission.emailThreats.post(request_body = request_body)


```