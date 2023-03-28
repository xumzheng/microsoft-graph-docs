---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InferenceClassificationOverride();
$requestBody.setClassifyAs(new InferenceClassificationType('focused'));



$requestResult = $graphServiceClient.me().inferenceClassification().overridesById('inferenceClassificationOverride-id').patch($requestBody);


```