---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = VersionsRequestBuilderGetRequestConfiguration(
request_config = VersionsRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["category","displayName","versionNumber"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').versions.get(request_config, headers=request_config)


```