---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = VersionsRequestBuilderGetRequestConfiguration();

query_params = VersionsRequestBuilderGetQueryParameters();
query_params.select = ["category","displayName","versionNumber"];

request_config.queryParameters = query_params;


result = awaitclient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').versions().get(request_config);


```