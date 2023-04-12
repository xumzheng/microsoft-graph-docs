---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCaseSettings()
request_body.@odatatype = '#microsoft.graph.security.ediscoveryCaseSettings'

redundancyDetection = RedundancyDetectionSettings()
redundancyDetection.@odatatype = 'microsoft.graph.security.redundancyDetectionSettings'


request_body.redundancyDetection = redundancyDetection
topicModeling = TopicModelingSettings()
topicModeling.@odatatype = 'microsoft.graph.security.topicModelingSettings'


request_body.topicModeling = topicModeling
ocr = OcrSettings()
ocr.@odatatype = 'microsoft.graph.security.ocrSettings'


request_body.ocr = ocr



result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').settings.patch(request_body = request_body)


```