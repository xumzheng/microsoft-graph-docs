---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = InferenceClassificationOverride();
request_body.setClassifyAs(InferenceClassificationType('focused'));

senderEmailAddress = EmailAddress();
senderEmailAddress.setName('Samantha Booth');

senderEmailAddress.setAddress('samanthab@adatum.onmicrosoft.com');


request_body.setSenderEmailAddress($senderEmailAddress);


result = await client.me().inferenceClassification().overrides().post(request_body);


```