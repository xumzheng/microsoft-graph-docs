---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InferenceClassificationOverride()
request_body.ClassifyAs(InferenceClassificationType('focused'))

sender_email_address = EmailAddress()
senderEmailAddress.name = 'Samantha Booth'

senderEmailAddress.address = 'samanthab@adatum.onmicrosoft.com'


request_body.sender_email_address = senderEmailAddress



result = await client.me.inferenceClassification.overrides.post(request_body = request_body)


```