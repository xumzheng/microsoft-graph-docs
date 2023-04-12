---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyTagsPostRequestBody()
tagsToAddEdiscoveryReviewTag1 = EdiscoveryReviewTag()
tagsToAddEdiscoveryReviewTag1.id = 'd3d99dc704a74801b792b3e1e722aa0d'


tagsToAddArray []= tagsToAddEdiscoveryReviewTag1;
request_body.tagstoadd(tagsToAddArray)





await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').reviewSets_by_id('ediscoveryReviewSet-id').queries_by_id('ediscoveryReviewSetQuery-id').securityapplyTags.post(request_body = request_body)


```