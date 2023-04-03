---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ApplyTagsPostRequestBody();
tagsToAddTag1 = Tag();
tagsToAddTag1.setId('b4798d14-748d-468e-a1ec-96a2b1d49677');


tagsToAddArray []= tagsToAddTag1;
requestBody.setTagsToAdd(tagsToAddArray);




awaitclient.compliance().ediscovery().casesById('case-id').reviewSetsById('reviewSet-id').queriesById('reviewSetQuery-id').ediscoveryApplyTags().post(requestBody);


```