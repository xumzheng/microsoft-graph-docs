---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ListItemRequestBuilderGetRequestConfiguration();

query_params = ListItemRequestBuilderGetQueryParameters();
query_params.expand = ["fields"];

request_config.queryParameters = query_params;


result = awaitclient.sitesById('site-id').listsById('list-id').itemsById('listItem-id').get(request_config);


```