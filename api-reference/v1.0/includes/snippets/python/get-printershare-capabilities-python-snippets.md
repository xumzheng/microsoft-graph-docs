---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PrinterShareRequestBuilderGetRequestConfiguration();

query_params = PrinterShareRequestBuilderGetQueryParameters();
query_params.select = ["id","displayName","capabilities"];

request_config.queryParameters = query_params;


result = awaitclient.print().sharesById('printerShare-id').get(request_config);


```