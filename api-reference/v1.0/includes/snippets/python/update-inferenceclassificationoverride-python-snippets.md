---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = InferenceClassificationOverride();
requestBody.setClassifyAs(InferenceClassificationType('focused'));



result = await client.me().inferenceClassification().overridesById('inferenceClassificationOverride-id').patch(requestBody);


```