---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = GroupRequestBuilderGetRequestConfiguration();

query_params = GroupRequestBuilderGetQueryParameters();
query_params.select = ["*","parentSiteId"];

request_config.queryParameters = query_params;


result = awaitclient.sitesById('site-id').termStore().groupsById('group-id').get(request_config);


```