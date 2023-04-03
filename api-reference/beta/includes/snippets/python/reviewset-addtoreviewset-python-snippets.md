---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AddToReviewSetPostRequestBody();
sourceCollection = SourceCollection();
sourceCollection.setId('1a9b4145d8f84e39bc45a7f68c5c5119');


requestBody.setSourceCollection($sourceCollection);
additionalData = [
'additionalData' => 'linkedFiles', 
];
requestBody.setAdditionalData(additionalData);




await client.compliance().ediscovery().casesById('case-id').reviewSetsById('reviewSet-id').ediscoveryAddToReviewSet().post(requestBody);


```