---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Inference_classification_override()
request_body.classifyas(InferenceClassificationType.Focused('inferenceclassificationtype.focused'))

sender_email_address = Email_address()
sender_email_address.name = 'Samantha Booth'

sender_email_address.address = 'samanthab@adatum.onmicrosoft.com'


request_body.sender_email_address = sender_email_address



result = await client.me.inference_classification.overrides.post(request_body = request_body)


```