---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = VlookupPostRequestBody()
request_body.lookupValue = 'pear'

table_array = Json()
additionalData = [
'Address' => 'Sheet1!B2:C7', 
];
tableArray.additionaldata(additionalData)



request_body.table_array = tableArray
request_body.col_index_num = 2

request_body.range_lookup = False



request_configuration = VlookupRequestBuilder.VlookupRequestBuilderPostRequestConfiguration(
headers = {
		'workbook-session-id' : "{session-id}",
}

)


result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.functions.vlookup.post(request_body = request_body, request_configuration = request_configuration)


```