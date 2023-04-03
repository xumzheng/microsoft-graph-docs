---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EvaluateClassificationResultsPostRequestBody();
contentInfo = ContentInfo();
contentInfo.set@odatatype('#microsoft.graph.contentInfo');

contentInfo.setFormat(ContentFormat('default'));

ContentInfo.setIdentifier(null);

contentInfo.setState(ContentState('rest'));

additionalData = [
'format@odata.type' => '#microsoft.graph.contentFormat', 
'state@odata.type' => '#microsoft.graph.contentState', 
];
contentInfo.setAdditionalData(additionalData);



requestBody.setContentInfo($contentInfo);
classificationResultsClassificationResult1 = ClassificationResult();
classificationResultsClassificationResult1.setSensitiveTypeId('cb353f78-2b72-4c3c-8827-92ebe4f69fdf');

classificationResultsClassificationResult1.setCount(4);

classificationResultsClassificationResult1.setConfidenceLevel(75);


classificationResultsArray []= classificationResultsClassificationResult1;
requestBody.setClassificationResults(classificationResultsArray);



requestConfiguration = EvaluateClassificationResultsRequestBuilderPostRequestConfiguration();

headers = [
'User-Agent' => 'ContosoLOBApp/1.0',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.informationProtection().policy().labels().evaluateClassificationResults().post(requestBody, requestConfiguration);


```