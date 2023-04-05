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




await client.compliance_ediscovery_casesby_id('case-id')_reviewSetsby_id('reviewSet-id')_queriesby_id('reviewSetQuery-id')_ediscoveryapplyTags.post(request_body)


```