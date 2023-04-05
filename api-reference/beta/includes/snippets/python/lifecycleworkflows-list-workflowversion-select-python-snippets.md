---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = VersionsRequestBuilderGetRequestConfiguration()

query_params = VersionsRequestBuilderGetQueryParameters()
query_params.select = ["category","displayName","versionNumber"]

request_config.queryParameters = query_params


result = await client.identityGovernance_lifecycleWorkflows_workflowsby_id('workflow-id')_versions.get(request_config)


```