---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyTagsPostRequestBody()
tagsToAddEdiscoveryReviewTag1 = EdiscoveryReviewTag()
tagsToAddEdiscoveryReviewTag1.setId('d3d99dc704a74801b792b3e1e722aa0d')


tagsToAddArray []= tagsToAddEdiscoveryReviewTag1;
request_body.setTagsToAdd(tagsToAddArray)




await client.security.cases.ediscoveryCases._by_id('ediscoveryCase-id').reviewSets._by_id('ediscoveryReviewSet-id').queries._by_id('ediscoveryReviewSetQuery-id').securityapplyTags.post(request_body)


```