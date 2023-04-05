---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TagRequestBuilderDeleteRequestConfiguration(
query_params = TagRequestBuilderDeleteQueryParameters()
query_params.forcedelete = true

)


await client.compliance.ediscovery.cases_by_id('case-id').tags_by_id('tag-id').delete(request_config)


```