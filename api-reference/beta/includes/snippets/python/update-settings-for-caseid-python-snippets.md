---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CaseSettings()
redundancyDetection = RedundancyDetectionSettings()
redundancyDetection.setIsEnabled(false)

redundancyDetection.setSimilarityThreshold(70)

redundancyDetection.setMinWords(12)

redundancyDetection.setMaxWords(400000)


request_body.setRedundancyDetection($redundancyDetection)
topicModeling = TopicModelingSettings()
topicModeling.setIsEnabled(false)

topicModeling.setIgnoreNumbers(false)

topicModeling.setTopicCount(50)

topicModeling.setDynamicallyAdjustTopicCount(false)


request_body.setTopicModeling($topicModeling)
ocr = OcrSettings()
ocr.setIsEnabled(true)

ocr.setMaxImageSize(12000)


request_body.setOcr($ocr)


result = await client.compliance.ediscovery.cases_by_id('case-id').settings.patch(request_body, headers=)


```