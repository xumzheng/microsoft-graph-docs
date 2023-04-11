---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddToReviewSetPostRequestBody()
search = EdiscoverySearch()
search.id = 'c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7'


request_body.search = search
request_body.AdditionalDataOptions(AdditionalDataOptions('linkedfiles'))



request_configuration = AddToReviewSetRequestBuilderPostRequestConfiguration(
)


await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').reviewSets_by_id('ediscoveryReviewSet-id').securityaddToReviewSet.post(request_body = request_body)


```