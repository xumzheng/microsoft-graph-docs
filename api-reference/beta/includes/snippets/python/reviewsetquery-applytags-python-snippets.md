---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyTagsPostRequestBody()
tagsToAddTag1 = Tag()
tagsToAddTag1.setId('b4798d14-748d-468e-a1ec-96a2b1d49677')


tagsToAddArray []= tagsToAddTag1;
request_body.setTagsToAdd(tagsToAddArray)




await client.compliance.ediscovery.cases._by_id('case-id').reviewSets._by_id('reviewSet-id').queries._by_id('reviewSetQuery-id').ediscoveryapplyTags.post(request_body)


```