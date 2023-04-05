---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddToReviewSetPostRequestBody()
search = EdiscoverySearch()
search.setId('c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7')


request_body.setSearch($search)
request_body.setAdditionalDataOptions(AdditionalDataOptions('linkedfiles'))



await client.security.cases.ediscoveryCasesby_id('ediscoveryCase-id').reviewSetsby_id('ediscoveryReviewSet-id').securityaddToReviewSet.post(request_body)


```