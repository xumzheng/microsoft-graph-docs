---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PrinterShareRequestBuilderGetRequestConfiguration(
request_configuration = PrinterShareRequestBuilderGetRequestConfiguration(query_params=query_params = PrinterShareRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","capabilities"]

)
query_params = PrinterShareRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","capabilities"]

)


result = await client.print.shares_by_id('printerShare-id').get(request_configuration)


```