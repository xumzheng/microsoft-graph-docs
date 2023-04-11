---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InferenceClassificationOverride()
request_body.ClassifyAs(InferenceClassificationType('focused'))




result = await client.me.inferenceClassification.overrides_by_id('inferenceClassificationOverride-id').patch(request_body = request_body)


```