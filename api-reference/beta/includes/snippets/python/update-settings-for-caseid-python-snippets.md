---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CaseSettings()
redundancy_detection = RedundancyDetectionSettings()
redundancyDetection.is_enabled = False

redundancyDetection.similarity_threshold = 70

redundancyDetection.min_words = 12

redundancyDetection.max_words = 400000


request_body.redundancy_detection = redundancyDetection
topic_modeling = TopicModelingSettings()
topicModeling.is_enabled = False

topicModeling.ignore_numbers = False

topicModeling.topic_count = 50

topicModeling.dynamically_adjust_topic_count = False


request_body.topic_modeling = topicModeling
ocr = OcrSettings()
ocr.is_enabled = True

ocr.max_image_size = 12000


request_body.ocr = ocr



result = await client.compliance.ediscovery.cases_by_id('case-id').settings.patch(request_body = request_body)


```