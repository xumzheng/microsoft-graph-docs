---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TagRequestBuilder.TagRequestBuilderDeleteQueryParameters(
				forcedelete = true,
)

request_configuration = TagRequestBuilderDeleteRequestConfiguration(
query_parameters = query_params,
)


await client.compliance.ediscovery.cases_by_id('case-id').tags_by_id('tag-id').delete(request_configuration = request_configuration)


```