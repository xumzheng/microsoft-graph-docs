---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = InferenceClassificationOverride();
requestBody.setClassifyAs(InferenceClassificationType('focused'));

senderEmailAddress = EmailAddress();
senderEmailAddress.setName('Samantha Booth');

senderEmailAddress.setAddress('samanthab@adatum.onmicrosoft.com');


requestBody.setSenderEmailAddress($senderEmailAddress);


requestResult = graphServiceClient.me().inferenceClassification().overrides().post(requestBody);


```