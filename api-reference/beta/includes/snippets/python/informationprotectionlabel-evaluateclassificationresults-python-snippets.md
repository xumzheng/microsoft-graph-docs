---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EvaluateClassificationResultsPostRequestBody()
contentInfo = ContentInfo()
contentInfo.set@odatatype('#microsoft.graph.contentInfo')

contentInfo.setFormat(ContentFormat('default'))

ContentInfo.setIdentifier(null)

contentInfo.setState(ContentState('rest'))

additionalData = [
'format@odata.type' => '#microsoft.graph.contentFormat', 
'state@odata.type' => '#microsoft.graph.contentState', 
];
contentInfo.setAdditionalData(additionalData)



request_body.setContentInfo($contentInfo)
classificationResultsClassificationResult1 = ClassificationResult()
classificationResultsClassificationResult1.setSensitiveTypeId('cb353f78-2b72-4c3c-8827-92ebe4f69fdf')

classificationResultsClassificationResult1.setCount(4)

classificationResultsClassificationResult1.setConfidenceLevel(75)


classificationResultsArray []= classificationResultsClassificationResult1;
request_body.setClassificationResults(classificationResultsArray)



request_config = EvaluateClassificationResultsRequestBuilderPostRequestConfiguration()

headers = [
'User-Agent' => 'ContosoLOBApp/1.0',
]

request_config.headers = headers


result = await client.informationProtection.policy.labels.evaluateClassificationResults.post(request_body, request_config)


```