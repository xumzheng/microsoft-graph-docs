---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PrinterRequestBuilderGetRequestConfiguration();

query_params = PrinterRequestBuilderGetQueryParameters();
query_params.select = ["id","displayName","capabilities"];

request_config.queryParameters = query_params;


result = awaitclient.print().printersById('printer-id').get(request_config);


```