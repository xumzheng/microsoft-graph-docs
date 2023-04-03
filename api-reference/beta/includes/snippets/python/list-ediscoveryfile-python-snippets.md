---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = FilesRequestBuilderGetRequestConfiguration();

queryParameters = FilesRequestBuilderGetQueryParameters();
queryParameters.top = 5;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').files().get(requestConfiguration);


```