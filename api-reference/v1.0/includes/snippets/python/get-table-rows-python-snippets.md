---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RowsRequestBuilder.RowsRequestBuilderGetQueryParameters(
		top = 5,
		skip = 5,
)

request_configuration = RowsRequestBuilder.RowsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').rows.get(request_configuration = request_configuration)


```