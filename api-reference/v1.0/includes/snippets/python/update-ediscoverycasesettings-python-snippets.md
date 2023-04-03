---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryCaseSettings();
requestBody.set@odatatype('#microsoft.graph.security.ediscoveryCaseSettings');

redundancyDetection = RedundancyDetectionSettings();
redundancyDetection.set@odatatype('microsoft.graph.security.redundancyDetectionSettings');


requestBody.setRedundancyDetection($redundancyDetection);
topicModeling = TopicModelingSettings();
topicModeling.set@odatatype('microsoft.graph.security.topicModelingSettings');


requestBody.setTopicModeling($topicModeling);
ocr = OcrSettings();
ocr.set@odatatype('microsoft.graph.security.ocrSettings');


requestBody.setOcr($ocr);


requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').settings().patch(requestBody);


```