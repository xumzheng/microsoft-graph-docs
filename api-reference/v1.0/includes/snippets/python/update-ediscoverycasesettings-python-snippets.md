---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EdiscoveryCaseSettings()
request_body.set@odatatype('#microsoft.graph.security.ediscoveryCaseSettings')

redundancyDetection = RedundancyDetectionSettings()
redundancyDetection.set@odatatype('microsoft.graph.security.redundancyDetectionSettings')


request_body.setRedundancyDetection($redundancyDetection)
topicModeling = TopicModelingSettings()
topicModeling.set@odatatype('microsoft.graph.security.topicModelingSettings')


request_body.setTopicModeling($topicModeling)
ocr = OcrSettings()
ocr.set@odatatype('microsoft.graph.security.ocrSettings')


request_body.setOcr($ocr)


result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').settings.patch(request_body)


```