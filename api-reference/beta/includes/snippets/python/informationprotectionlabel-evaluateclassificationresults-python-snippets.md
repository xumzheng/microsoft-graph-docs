---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EvaluateClassificationResultsPostRequestBody()
contentInfo = ContentInfo()
contentInfo.@odatatype = '#microsoft.graph.contentInfo'

contentInfo.Format(ContentFormat('default'))

ContentInfo.identifier=null

contentInfo.State(ContentState('rest'))

additionalData = [
'format@odata.type' => '#microsoft.graph.contentFormat', 
'state@odata.type' => '#microsoft.graph.contentState', 
];
contentInfo.additionaldata(additionalData)



request_body.contentInfo = contentInfo
classificationResultsClassificationResult1 = ClassificationResult()
classificationResultsClassificationResult1.sensitiveTypeId = 'cb353f78-2b72-4c3c-8827-92ebe4f69fdf'

classificationResultsClassificationResult1.count = 4

classificationResultsClassificationResult1.confidenceLevel = 75


classificationResultsArray []= classificationResultsClassificationResult1;
request_body.classificationresults(classificationResultsArray)



headers = {
'User-Agent' : "ContosoLOBApp/1.0",
}

)


result = await client.informationProtection.policy.labels.evaluateClassificationResults.post(request_body = request_body, request_configuration = request_configuration)


```