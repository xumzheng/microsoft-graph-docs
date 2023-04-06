---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = VersionsRequestBuilderGetRequestConfiguration(
request_configuration = VersionsRequestBuilderGetRequestConfiguration(query_params=query_params = VersionsRequestBuilderGetQueryParameters()
query_params['select'] = ["category","displayName","versionNumber"]

)
query_params = VersionsRequestBuilderGetQueryParameters()
query_params['select'] = ["category","displayName","versionNumber"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').versions.get(request_configuration)


```