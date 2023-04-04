---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TagRequestBuilderDeleteRequestConfiguration();

query_params = TagRequestBuilderDeleteQueryParameters;
query_params.forcedelete = true;

request_config.queryParameters = query_params;


await client.compliance().ediscovery().casesById('case-id').tagsById('tag-id').delete(request_config);


```