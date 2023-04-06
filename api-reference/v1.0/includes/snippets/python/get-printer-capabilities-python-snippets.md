---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PrinterRequestBuilderGetRequestConfiguration(
request_config = PrinterRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","displayName","capabilities"]
)


result = await client.print.printers_by_id('printer-id').get(request_config, headers=request_config)


```