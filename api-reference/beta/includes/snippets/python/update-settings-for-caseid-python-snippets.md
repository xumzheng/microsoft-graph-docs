---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CaseSettings();
redundancyDetection = RedundancyDetectionSettings();
redundancyDetection.setIsEnabled(false);

redundancyDetection.setSimilarityThreshold(70);

redundancyDetection.setMinWords(12);

redundancyDetection.setMaxWords(400000);


requestBody.setRedundancyDetection($redundancyDetection);
topicModeling = TopicModelingSettings();
topicModeling.setIsEnabled(false);

topicModeling.setIgnoreNumbers(false);

topicModeling.setTopicCount(50);

topicModeling.setDynamicallyAdjustTopicCount(false);


requestBody.setTopicModeling($topicModeling);
ocr = OcrSettings();
ocr.setIsEnabled(true);

ocr.setMaxImageSize(12000);


requestBody.setOcr($ocr);


result = await client.compliance().ediscovery().casesById('case-id').settings().patch(requestBody);


```