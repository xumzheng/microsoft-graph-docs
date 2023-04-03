---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = DefinitionsRequestBuilderGetRequestConfiguration();

query_params = DefinitionsRequestBuilderGetQueryParameters();
query_params.filter = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')";

request_config.queryParameters = query_params;


result = awaitclient.identityGovernance().accessReviews().definitions().get(request_config);


```