---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddToReviewSetPostRequestBody()
sourceCollection = SourceCollection()
sourceCollection.setId('1a9b4145d8f84e39bc45a7f68c5c5119')


request_body.setSourceCollection($sourceCollection)
additionalData = [
'additionalData' => 'linkedFiles', 
];
request_body.setAdditionalData(additionalData)




await client.compliance.ediscovery.cases_by_id('case-id').reviewSets_by_id('reviewSet-id').ediscoveryaddToReviewSet.post(request_body)


```