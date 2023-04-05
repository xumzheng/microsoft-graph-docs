---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PrinterShareRequestBuilderGetRequestConfiguration(
query_params = PrinterShareRequestBuilderGetQueryParameters()
query_params.select = ["id","displayName","capabilities"]

)


result = await client.print.shares_by_id('printerShare-id').get(request_config)


```