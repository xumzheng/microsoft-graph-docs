---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCaseSettings()
request_body.@odatatype = '#microsoft.graph.security.ediscoveryCaseSettings'

redundancy_detection = RedundancyDetectionSettings()
redundancyDetection.@odatatype = 'microsoft.graph.security.redundancyDetectionSettings'


request_body.redundancy_detection = redundancyDetection
topic_modeling = TopicModelingSettings()
topicModeling.@odatatype = 'microsoft.graph.security.topicModelingSettings'


request_body.topic_modeling = topicModeling
ocr = OcrSettings()
ocr.@odatatype = 'microsoft.graph.security.ocrSettings'


request_body.ocr = ocr



result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').settings.patch(request_body = request_body)


```