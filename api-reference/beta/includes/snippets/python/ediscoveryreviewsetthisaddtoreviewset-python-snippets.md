---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddToReviewSetPostRequestBody();
search = EdiscoverySearch();
search.setId('c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7');


requestBody.setSearch($search);
requestBody.setAdditionalDataOptions(AdditionalDataOptions('linkedfiles'));



graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').securityAddToReviewSet().post(requestBody);


```