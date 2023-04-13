---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyPostRequestBody()
fields_workbook_sort_field1 = WorkbookSortField()
fieldsWorkbookSortField1.key = 99

fieldsWorkbookSortField1.sortOn = 'sortOn-value'

fieldsWorkbookSortField1.ascending = True

fieldsWorkbookSortField1.color = 'color-value'

fieldsWorkbookSortField1.dataOption = 'dataOption-value'

fields_workbook_sort_field1_icon = WorkbookIcon()
fieldsWorkbookSortField1Icon.set = 'set-value'

fieldsWorkbookSortField1Icon.index = 99


fieldsWorkbookSortField1.icon = fieldsWorkbookSortField1Icon

fieldsArray []= fieldsWorkbookSortField1;
request_body.fields(fieldsArray)


request_body.match_case = True

request_body.method = 'method-value'




await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').sort.apply.post(request_body = request_body)


```