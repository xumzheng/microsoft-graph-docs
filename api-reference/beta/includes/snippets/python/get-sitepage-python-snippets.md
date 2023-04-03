---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SitePageRequestBuilderGetRequestConfiguration();

query_params = SitePageRequestBuilderGetQueryParameters();
query_params.select = ["id","title"];
query_params.expand = ["webparts"];

request_config.queryParameters = query_params;


result = awaitclient.sitesById('site-id').pagesById('sitePage-id').get(request_config);


```