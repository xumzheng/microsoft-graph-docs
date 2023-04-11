---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CaseSettings()
redundancyDetection = RedundancyDetectionSettings()
redundancyDetection.isEnabled = false

redundancyDetection.similarityThreshold = 70

redundancyDetection.minWords = 12

redundancyDetection.maxWords = 400000


request_body.redundancyDetection = redundancyDetection
topicModeling = TopicModelingSettings()
topicModeling.isEnabled = false

topicModeling.ignoreNumbers = false

topicModeling.topicCount = 50

topicModeling.dynamicallyAdjustTopicCount = false


request_body.topicModeling = topicModeling
ocr = OcrSettings()
ocr.isEnabled = true

ocr.maxImageSize = 12000


request_body.ocr = ocr



result = await client.compliance.ediscovery.cases_by_id('case-id').settings.patch(request_body = request_body)


```