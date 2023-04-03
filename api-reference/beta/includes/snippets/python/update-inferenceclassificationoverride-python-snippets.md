---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = InferenceClassificationOverride();
requestBody.setClassifyAs(InferenceClassificationType('focused'));



requestResult = graphServiceClient.me().inferenceClassification().overridesById('inferenceClassificationOverride-id').patch(requestBody);


```