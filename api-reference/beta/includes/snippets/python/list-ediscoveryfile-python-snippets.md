---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = FilesRequestBuilderGetRequestConfiguration();

query_params = FilesRequestBuilderGetQueryParameters();
query_params.top = 5;

request_config.queryParameters = query_params;


result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').files().get(request_config);


```