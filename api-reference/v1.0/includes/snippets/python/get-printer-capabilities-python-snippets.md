---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PrinterRequestBuilderGetRequestConfiguration(
request_configuration = PrinterRequestBuilderGetRequestConfiguration(query_params=query_params = PrinterRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","capabilities"]

)
query_params = PrinterRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","capabilities"]

)


result = await client.print.printers_by_id('printer-id').get(request_configuration)


```